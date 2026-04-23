# Assignment 2 — Wage Prediction with Regression Models

## Autor

- **Josep Gabriel Fornes Reynes**

## Descripción del proyecto

Este proyecto estudia cómo predecir el salario de trabajadores varones de la región atlántica de Estados Unidos utilizando el dataset **`Wage`** del paquete `ISLR`.

El foco del trabajo es comparar distintos **modelos de regresión** para entender qué variables explican mejor el salario y qué enfoque resulta más útil a nivel predictivo.

## Objetivo

Construir y evaluar varios modelos de regresión para predecir `wage` o `logwage`, analizando el impacto de variables como:

- edad,
- educación,
- estado civil,
- raza,
- tipo de trabajo,
- salud,
- seguro médico,
- y año del registro.

## Dataset

Se emplea el dataset **`Wage`** del paquete `ISLR`, con aproximadamente 3000 observaciones y 11 variables relacionadas con salarios y características sociodemográficas.

## Metodología

El trabajo compara varios enfoques:

### 1. Regresión lineal simple

Se analiza qué variable individual se relaciona mejor con el salario. La conclusión principal es que **educación** actúa como el predictor individual más fuerte.

### 2. Regresión lineal múltiple

Se combinan varias variables explicativas para mejorar la capacidad predictiva del modelo.

### 3. Transformaciones no lineales

Se introducen transformaciones como:

- `age²`
- `log(age)`

para capturar relaciones no estrictamente lineales entre edad y salario.

### 4. Comparación con otros enfoques

También se comenta el uso de regresión polinómica y se justifica por qué la regresión logística no es adecuada para este problema, ya que la variable objetivo es continua.

## Resultados principales

- La **educación** es la mejor variable individual para explicar el salario.
- El mejor rendimiento global se obtiene con la **regresión lineal múltiple**.
- Las transformaciones de edad mejoran ligeramente el ajuste, lo que sugiere que la relación entre edad y salario no es totalmente lineal.
- Los modelos polinómicos no aportan una mejora significativa respecto al enfoque múltiple.

## Tecnologías utilizadas

- **R**
- **R Markdown**
- **ISLR**
- funciones base de modelado (`lm`)

## Archivos principales

- `Assegnment2.Rmd`
- `Assegnment2.html`
- `21746-2425assignment2.pdf`

## Valor del proyecto

Este proyecto aporta valor porque demuestra:

- comprensión de **modelos de regresión**,
- capacidad para **seleccionar variables**,
- interpretación de métricas como **R-squared**,
- y criterio para decidir cuándo un modelo es o no adecuado para una tarea concreta.
