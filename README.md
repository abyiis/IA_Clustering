# 📊 iaupb_examen_04_clustering: Análisis de Clustering para Hábitos de Actividad Física Saludable

---

## 🚀 Descripción del Proyecto

Este repositorio contiene un notebook de Jupyter (`iaupb_examen_04_clustering.ipynb`) que aplica y compara tres algoritmos de **Clustering** (K-Means, Jerárquico, DBSCAN) para segmentar a 500 individuos en grupos basados en sus **Hábitos de Actividad Física y Salud**.

El objetivo es determinar el método de agrupamiento más robusto y adecuado para un sistema de **monitoreo de salud poblacional** a gran escala, concluyendo con una justificación del modelo seleccionado.

---

## 👤 Autor

* **Nombre:** Juan david parra sierra
* **ID:** 000475676

---

## 💾 Datos

El análisis se basa en el archivo `patrones_actividad_saludable.csv`, que contiene 500 registros y 5 atributos clave relacionados con la salud y actividad física:

| Atributo | Descripción |
| :--- | :--- |
| `pasos_diarios` | Nivel de movimiento cotidiano. |
| `horas_sueño` | Ciclo de sueño y recuperación. |
| `minutos_ejercicio` | Duración del ejercicio planificado (minutos). |
| `frecuencia_cardiaca_reposo` | Condición cardiovascular. |
| `calorias_quemadas` | Gasto energético diario total. |

---

## ⚙️ Flujo de Trabajo

El notebook sigue los siguientes pasos:

1.  **Carga y Exploración de Datos (EDA)**: Inspección inicial y limpieza.
2.  **Preprocesamiento**: Estandarización de las variables (`StandardScaler`).
3.  **Modelado y Evaluación**:
    * **K-Means**: Aplicación y uso del método del codo para determinar `k`.
    * **Clustering Jerárquico**: Análisis mediante dendrograma y `AgglomerativeClustering`.
    * **DBSCAN**: Optimización de parámetros (`eps` y `min_samples`).
4.  **Análisis de Resultados**: Comparación de la idoneidad de los tres modelos en el contexto de la salud pública.

---

## ✅ Conclusión Clave

El algoritmo más adecuado para un sistema real de **monitoreo de salud poblacional** es **DBSCAN**.

**Justificación:**

* **Robustez:** Identifica **ruido y *outliers*** (frecuentes en datos de salud) sin asignarlos a clusters principales.
* **Escalabilidad:** Puede manejar **grandes volúmenes de datos** mejor que el Clustering Jerárquico.
* **Flexibilidad:** No requiere pre-especificar el número de clusters (*k*) como K-Means.
* **Impacto en Salud Pública:** Permite detectar **grupos minoritarios** de alto riesgo que K-Means o el Jerárquico podrían agrupar erróneamente con la mayoría.

* ## 👤 Información del Autor

| **Nombre** | [juan david parra sierra] |
| **ID / Código** | [000475676] |
