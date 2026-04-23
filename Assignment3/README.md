# Assignment 3 — Loan Approval Classification

## Autores

- **Jordi Florit Ensenyat**
- **Josep Gabriel Fornés Reynés**
- **Pau Girón Rodríguez**

## Descripción del proyecto

Este proyecto aborda un problema clásico de **clasificación supervisada**: predecir si una solicitud de préstamo será aprobada o no a partir de variables relacionadas con el perfil financiero y laboral del solicitante.

El trabajo no se limita a entrenar un único modelo, sino que desarrolla un pipeline bastante completo que incluye:

- análisis exploratorio,
- tratamiento de valores perdidos y outliers,
- diferentes transformaciones del dataset,
- y comparación de varios algoritmos de clasificación.

## Objetivo

Construir modelos predictivos para clasificar `loan_status` y comparar cuál funciona mejor según diferentes configuraciones de preprocesado y representación de los datos.

## Dataset

Se utiliza un dataset de aprobación de préstamos inspirado en crédito de riesgo, con variables como:

- edad,
- ingresos,
- experiencia laboral,
- historial crediticio,
- importe solicitado,
- propósito del préstamo,
- y otras características financieras.

Archivos incluidos:

- `loan_data.csv`
- `loan_data_cleaned.csv`

## Metodología

### 1. Exploratory Data Analysis

Se revisa la estructura del dataset, la distribución de variables, correlaciones, valores faltantes y posibles valores atípicos.

### 2. Data preprocessing

Se aplican varias estrategias de preparación:

- limpieza de outliers,
- codificación de variables categóricas,
- normalización y estandarización,
- y evaluación del efecto de cada transformación sobre los modelos.

### 3. Modelos evaluados

En el proyecto se prueban varios clasificadores, entre ellos:

- **KNN**
- **Naive Bayes**
- **Decision Trees (`rpart`)**
- flujos de entrenamiento y validación con **`caret`**
- técnicas de balanceo como **SMOTE**

## Resultados y conclusiones

- El proyecto muestra una comparación real entre modelos y configuraciones, no solo un resultado aislado.
- Se observa que el preprocesado influye de forma clara en el rendimiento final.
- Los modelos basados en árboles y algunas configuraciones balanceadas destacan por ofrecer un mejor equilibrio entre precisión y capacidad de generalización.
- El trabajo alcanza resultados altos de accuracy en sus mejores configuraciones y también analiza métricas de equilibrio de clases, algo importante en problemas de riesgo.

## Tecnologías utilizadas

- **R**
- **R Markdown**
- `tidyverse`
- `ggplot2`
- `caret`
- `e1071`
- `rpart`
- `rpart.plot`
- `SMOTE`

## Archivos principales

- `Assignment3.Rmd`
- `Assignment3.html`
- `Assignment3.nb.html`
- `loan_data.csv`
- `loan_data_cleaned.csv`

## Valor del proyecto

Este trabajo es especialmente fuerte para portfolio porque enseña:

- diseño de un **pipeline de clasificación completo**,
- tratamiento realista de datos problemáticos,
- comparación de algoritmos,
- uso de métricas más allá de la accuracy,
- y enfoque práctico sobre un caso de negocio muy reconocible: **riesgo crediticio**.
