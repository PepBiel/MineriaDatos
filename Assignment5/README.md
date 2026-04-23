# Assignment 5 — Association Rules with Apriori and Eclat

## Autores

- **Jordi Florit Ensenyat**
- **Josep Gabriel Fornes Reynes**
- **Pau Girón Rodríguez**

## Descripción del proyecto

Este proyecto aplica técnicas de **minería de reglas de asociación** sobre un conjunto de transacciones reales de panadería. El objetivo es descubrir qué productos tienden a comprarse juntos y comparar dos algoritmos clásicos del área: **Apriori** y **Eclat**.

## Objetivo

Identificar itemsets frecuentes y generar reglas de asociación útiles para entender patrones de compra dentro del dataset `BreadBasket.csv`.

## Dataset

El proyecto utiliza el dataset **BreadBasket**, compuesto por transacciones reales de una bakery.

Cada transacción agrupa los productos comprados por un cliente en una misma operación, lo que lo convierte en un caso ideal para market basket analysis.

## Metodología

### 1. Preparación de datos transaccionales

Los datos se convierten al formato `transactions` del paquete `arules`, requisito necesario para aplicar los algoritmos de asociación.

### 2. Apriori

Se explora el algoritmo **Apriori** variando varios hiperparámetros:

- soporte,
- confianza,
- longitud mínima de regla.

Además, se eliminan reglas redundantes para quedarse con un conjunto más interpretable.

### 3. Eclat

Se evalúa **Eclat** como alternativa centrada en itemsets frecuentes y posterior inducción de reglas.

### 4. Comparación de calidad

Las reglas se comparan usando métricas como:

- **support**
- **confidence**
- **lift**

## Principales resultados

- El proyecto demuestra bien cómo cambian los resultados según la configuración de soporte y confianza.
- Se identifican combinaciones de parámetros más equilibradas para generar un número manejable de reglas útiles.
- Apriori y Eclat se comparan no solo a nivel técnico, sino también desde la interpretabilidad de las reglas obtenidas.
- El trabajo presta atención a la eliminación de redundancia, algo importante para convertir reglas en hallazgos realmente accionables.

## Tecnologías utilizadas

- **R**
- **R Markdown**
- `arules`

## Archivos principales

- `Assignment5.Rmd`
- `Assignment5.html`
- `BreadBasket.csv`

## Valor del proyecto

Este proyecto es muy interesante para portfolio porque conecta la minería de datos con un caso de negocio muy entendible:

- análisis de cesta de la compra,
- descubrimiento de patrones de consumo,
- recomendación de productos,
- y optimización de ventas cruzadas.
