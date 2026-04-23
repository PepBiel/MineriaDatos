# Final Practice — Real Estate Analysis in Portugal

## Autores

- **Antonio Torres Escribano**
- **Jaume Cantallops Comas**
- **Jordi Florit Ensenyat**
- **Josep Gabriel Fornes Reynes**
- **Pau Girón Rodríguez**

## Descripción del proyecto

Este proyecto final aborda un problema claramente orientado a negocio: **analizar el mercado inmobiliario en Portugal para identificar qué factores influyen en el precio y detectar propiedades potencialmente infravaloradas**.

Es el trabajo más completo del repositorio porque combina:

- limpieza y exploración de datos,
- análisis estadístico,
- regresión,
- clustering,
- y una lectura final enfocada a oportunidades de inversión.

## Objetivo

Responder a tres preguntas principales:

1. **Qué variables influyen más en el precio de una propiedad**.
2. **Qué características comparten las propiedades de mayor valor**.
3. **Qué zonas de Portugal concentran más propiedades infravaloradas**.

## Datasets

El proyecto trabaja con datos inmobiliarios de Portugal, diferenciando varios tipos de activos:

- apartamentos,
- casas,
- terrenos.

Archivos incluidos:

- `portugal_housing.csv`
- `dataset_limpio.csv`

## Metodología

### 1. Data cleaning y EDA

Se estudian valores faltantes, columnas vacías, variables con alto porcentaje de missing y distribuciones por tipo de propiedad. También se consolidan columnas equivalentes y se eliminan atributos poco útiles.

### 2. Análisis de factores que afectan al precio

Se estudia la relación entre el precio y variables como:

- superficie,
- número de baños,
- habitaciones,
- año de construcción,
- ascensor,
- parking,
- certificado energético,
- ciudad y distrito.

### 3. Modelos predictivos

Se aplican modelos de regresión para estimar precios esperados y comparar alternativas según métricas como:

- **R-squared**
- **RMSE**

### 4. Detección de propiedades infravaloradas

A partir de la diferencia entre precio real y precio estimado, se construye una lógica para identificar inmuebles que podrían estar por debajo de su valor esperado.

### 5. Clustering

Se aplica **K-Means** para agrupar propiedades con características similares y analizar clusters con mayor concentración de oportunidades.

### 6. Análisis geográfico

Se estudia qué distritos presentan mayor porcentaje de propiedades infravaloradas, diferenciando entre apartamentos, casas y terrenos.

## Principales hallazgos

- El proyecto identifica factores estructurales y de localización que afectan de forma clara al precio.
- La combinación de **regresión + clustering** permite pasar del análisis descriptivo a una lectura orientada a decisión.
- Se detectan distritos con mayor concentración de propiedades aparentemente infravaloradas, lo que convierte el análisis en una herramienta útil para inversión.
- El trabajo destaca especialmente por traducir técnicas de minería de datos a una pregunta de negocio concreta y muy comprensible.

## Tecnologías utilizadas

- **R**
- **R Markdown**
- `dplyr`
- `tidyr`
- `ggplot2`
- `ggcorrplot`
- `corrplot`
- `cluster`
- `gridExtra`

## Archivos principales

- `PracticaFinal.Rmd`
- `PracticaFinal.html`
- `portugal_housing.csv`
- `dataset_limpio.csv`

## Valor del proyecto

Este es probablemente el proyecto con más valor de portfolio dentro del repositorio porque demuestra:

- capacidad para trabajar con un problema de negocio real,
- combinación de varias técnicas de análisis,
- criterio para limpiar y transformar datos complejos,
- y enfoque final orientado a **insight accionable**.
