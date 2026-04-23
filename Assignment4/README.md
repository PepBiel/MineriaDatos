# Assignment 4 — Clustering Analysis on Penguin Data

## Autores

- **Jordi Florit Ensenyat**
- **Josep Gabriel Fornes Reynes**
- **Pau Girón Rodríguez**

## Descripción del proyecto

Este proyecto explora técnicas de **aprendizaje no supervisado** aplicadas a un dataset de pingüinos. El objetivo es descubrir agrupaciones naturales en los datos a partir de características morfológicas y categóricas.

Se trata de una práctica muy completa de clustering porque compara métodos de distinta naturaleza y analiza cómo cambia la segmentación según el algoritmo utilizado.

## Objetivo

Aplicar y comparar diferentes técnicas de clustering para identificar estructuras y patrones en el dataset `penguindata.csv`.

## Dataset

Se utiliza un dataset de pingüinos del archipiélago Palmer con variables como:

- longitud del pico,
- profundidad del pico,
- longitud de aleta,
- masa corporal,
- sexo,
- especie,
- isla.

## Metodología

### 1. Exploratory Data Analysis

Se estudian distribuciones, boxplots, valores faltantes y outliers para entender la estructura del dataset antes de agruparlo.

### 2. Preprocesado

Se limpian datos, se gestionan valores perdidos y se transforman variables cuando es necesario para poder aplicar algoritmos de clustering de forma consistente.

### 3. Algoritmos comparados

El proyecto evalúa varios enfoques:

- **AGNES** (clustering jerárquico)
- **K-Means**
- **PAM**
- **DBSCAN**
- y métodos adicionales relacionados con segmentación y visualización

### 4. Evaluación de la calidad de clusters

Se utilizan visualizaciones, dendrogramas, análisis de separación y medidas como el **silhouette width** para comparar configuraciones.

## Conclusiones principales

- **AGNES** permite identificar una estructura jerárquica clara y útil para interpretar relaciones entre observaciones.
- **K-Means** ofrece una segmentación eficiente y compacta, especialmente con 4 clusters.
- **PAM** resulta más robusto frente a outliers que K-Means.
- **DBSCAN** aporta valor para detectar ruido y puntos atípicos.
- La práctica destaca por comparar métodos con supuestos distintos, lo que da una visión muy completa del problema.

## Tecnologías utilizadas

- **R**
- **R Markdown**
- `ggplot2`
- `dplyr`
- `patchwork`
- `GGally`
- `dendextend`
- `dbscan`
- `factoextra`
- `mclust`

## Archivos principales

- `Assignment4.Rmd`
- `Assignment4.html`
- `penguindata.csv`

## Valor del proyecto

Este proyecto es muy útil para mostrar capacidad en:

- **clustering y segmentación**, 
- comparación entre enfoques supervisados y no supervisados,
- interpretación de resultados no triviales,
- y uso de visualización para justificar decisiones analíticas.
