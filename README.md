#Telecom X: Predicción de Evasión de Clientes

Este repositorio contiene un análisis de datos y modelado predictivo para identificar clientes en riesgo de abandonar la compañía **Telecom X**. El proyecto se divide en dos fases: limpieza y análisis descriptivo, seguido de un proceso de balanceo de clases y entrenamiento de modelos de Machine Learning.

##Resumen del Proyecto

El objetivo principal fue entender por qué los clientes se van y construir un sistema que anticipe estas salidas. Tras el procesamiento, el modelo seleccionado permite detectar al **82% de los clientes con intención de fuga**, brindando una herramienta clave para campañas de retención.

##Tecnologías y Metodología
* **Lenguaje:** Python (Google Colab)
* **Librerías Clave:** Pandas, Scikit-Learn, Seaborn, Matplotlib, Imbalanced-learn (SMOTE).
* **Técnicas:** * Normalización de JSON anidados.
    * Balanceo de clases mediante sobremuestreo sintético (**SMOTE**).
    * Escalado de variables numéricas con **StandardScaler**.

##Hallazgos Clave (Insights)
* **Factor Tiempo:** Los clientes nuevos son los más vulnerables; el riesgo de fuga se concentra en los primeros **18 meses**.
* **Factor Costo:** El grupo que cancela paga un promedio de **~$74.44**, un 20% más que los clientes leales.
* **Contratos:** Los planes **"Month-to-month"** presentan la mayor tasa de rotación.

##Evaluación de Modelos
Se compararon dos algoritmos con naturalezas distintas:

1. **Regresión Logística (Seleccionado):** - **Recall:** 82% 
   - **Justificación:** Es el modelo más sensible para detectar casos positivos de Churn, minimizando las pérdidas por clientes no identificados.
2. **Random Forest:** - **Exactitud:** ~79%
   - **Observación:** Presentó signos de *overfitting*, memorizando los datos de entrenamiento pero perdiendo precisión en el test.

---
Proyecto desarrollado por floydCL como parte del Challenge de Data Science - Alura Latam.
