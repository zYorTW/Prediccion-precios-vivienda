# Predicción de Precios de Vivienda

Proyecto de análisis de datos para predecir el precio de propiedades inmobiliarias utilizando técnicas de machine learning.

## Objetivo del proyecto
Desarrollar un modelo capaz de estimar el precio de viviendas en función de sus características estructurales.

## Proceso

- Análisis exploratorio de datos (EDA)
- Limpieza y preprocesamiento
- Transformación logarítmica del precio
- Entrenamiento de modelos (Regresión Lineal y Random Forest)
- Evaluación con métricas (RMSE y R²)

## Resultados

- R²: 0.89 (Regresión Lineal)
- RMSE: 0.13
- Variable más influyente: OverallQual (~54%)

## Tecnologías

- Python
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## Conclusión

El modelo logró explicar el 89% de la variabilidad del precio de viviendas, siendo la calidad general de la propiedad el factor más determinante.

## Análisis Clave

- La variable **OverallQual** tiene la mayor influencia en el precio (~54%)
- El tamaño habitable (**GrLivArea**) es el segundo factor más relevante
- Se identificaron y eliminaron outliers que afectaban el rendimiento del modelo
- La transformación logarítmica mejoró la distribución del precio y el desempeño

## Modelos Evaluados

| Modelo            | R²     | RMSE   |
|------------------|--------|--------|
| Regresión Lineal | 0.892  | 0.130  |
| Random Forest    | 0.858  | 0.149  |

## Decisión

Se seleccionó la **Regresión Lineal** como modelo final debido a su mejor desempeño en métricas.

