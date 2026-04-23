# Assignment 1 — Exploratory Analysis and Manual Statistics with ChickWeight

## Autor

- **Josep Gabriel Fornés Reynés**

## Descripción del proyecto

Este proyecto realiza una primera aproximación práctica al análisis de datos en R utilizando el dataset **`ChickWeight`**. El trabajo combina dos bloques:

1. **Visualización exploratoria de datos**, para entender cómo evoluciona el peso de los pollos según el tiempo y la dieta.
2. **Cálculo manual de estadísticos**, evitando funciones estadísticas integradas de R para calcular media, varianza y covarianza.

El objetivo no es solo obtener resultados, sino demostrar comprensión de los fundamentos estadísticos y de la interpretación gráfica.

## Dataset

Se utiliza el dataset incorporado en R **`ChickWeight`**, que incluye:

- `weight`: peso del pollo
- `Time`: días de vida
- `Chick`: identificador del pollo
- `Diet`: tipo de dieta

## Qué se hizo

### 1. Análisis exploratorio

Se construyen tres visualizaciones para estudiar el comportamiento del dataset:

- **Line chart multigrupo** para observar la evolución del peso a lo largo del tiempo.
- **Boxplot** para comparar la distribución del peso por tipo de dieta.
- **Stacked bar chart** para analizar proporciones de categorías de peso según la dieta.

### 2. Estadística descriptiva sin funciones predefinidas

Se implementan manualmente las fórmulas de:

- media,
- varianza,
- covarianza.

Esto permite mostrar dominio de los conceptos matemáticos que hay detrás de las funciones automáticas del lenguaje.

## Principales conclusiones

- La **dieta influye claramente** en la evolución del peso de los pollos.
- Algunas dietas parecen producir mayor crecimiento y otras muestran más dispersión.
- El trabajo también identifica una limitación metodológica importante: calcular estadísticos sobre todas las observaciones mezcladas puede no ser la mejor decisión, porque cada pollo tiene múltiples mediciones a lo largo del tiempo.
- Como reflexión final, se propone que una alternativa más rigurosa sería trabajar con la **última observación de cada pollo**.

## Tecnologías utilizadas

- **R**
- **R Markdown**
- **ggplot2**

## Archivos principales

- `Assigment1.Rmd` — desarrollo completo del análisis
- `Assigment1.html` — versión renderizada
- `21746-2425assignment1.pdf` — enunciado o material de apoyo

## Valor del proyecto

Este trabajo es especialmente útil como pieza de portfolio porque demuestra:

- base sólida en **análisis exploratorio**,
- comprensión de **estadística descriptiva**,
- capacidad para **interpretar gráficos**,
- y criterio crítico para detectar limitaciones en el propio análisis.
