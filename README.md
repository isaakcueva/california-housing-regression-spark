# California Housing Regression with Apache Spark

Este proyecto implementa modelos de regresión lineal multivariable para predecir la mediana del valor de las viviendas en California utilizando Apache Spark.

## Descripción

Se trabaja con un dataset que contiene información geográfica, demográfica y socioeconómica de bloques en California, incluyendo variables como longitud, latitud, edad media de la vivienda, número total de habitaciones, ingreso medio, y proximidad al océano.

Las actividades principales incluyen:

- Limpieza de datos y tratamiento de valores faltantes (imputación con mediana).
- Codificación de variables categóricas mediante One-Hot Encoding.
- División del dataset en conjuntos de entrenamiento y evaluación.
- Creación y evaluación de un modelo de regresión lineal simple.
- Implementación y evaluación de modelos con regularización Lasso y Ridge.
- Comparación de los modelos y análisis de resultados.

## Tecnologías usadas

- Apache Spark (PySpark)
- Python 3
- Google Colab (entorno de ejecución)

## Resultados principales

| Modelo                    | MSE              | R²           |
|---------------------------|------------------|--------------|
| Regresión Lineal Simple    | 5,010,754,518.01 | 0.6378       |
| Regresión Lineal con Lasso | 5,153,100,102.19 | 0.6276       |
| Regresión Lineal con Ridge | 5,154,029,304.25 | 0.6275       |

## Conclusiones

Aunque el modelo lineal simple presenta un mejor ajuste según las métricas, los modelos con regularización (Lasso y Ridge) ofrecen mejor robustez y capacidad de generalización, ayudando a prevenir el sobreajuste. Se recomienda el modelo Lasso por su capacidad para simplificar el modelo seleccionando variables relevantes.

## Uso

Para ejecutar este proyecto, es necesario contar con un entorno con Apache Spark configurado, preferiblemente Google Colab con PySpark instalado.

Se recomienda seguir el notebook paso a paso para replicar el análisis.

---



