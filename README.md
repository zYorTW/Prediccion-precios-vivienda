## Autor

Yorland Insignares Escorcia  
Analista de Datos / Machine Learning  

# Predicción de Precios de Vivienda

Modelo de machine learning para estimar el precio de propiedades inmobiliarias a partir de variables estructurales y de calidad.

## Objetivo

Desarrollar un modelo capaz de predecir el precio de viviendas y analizar los factores que más influyen en su valor.

## Proceso

- Análisis exploratorio de datos (EDA) para identificar patrones y correlaciones
- Limpieza y preprocesamiento de datos (manejo de nulos y outliers)
- Transformación logarítmica de la variable objetivo para mejorar la distribución
- Codificación de variables categóricas mediante one-hot encoding
- Entrenamiento y evaluación de modelos de regresión

## Resultados

- **R²:** 0.892 (Regresión Lineal)
- **RMSE:** 0.130 (escala logarítmica)
- **Variable más influyente:** OverallQual (~54%)

## Análisis Clave

- **OverallQual** es el factor más determinante en el precio de la vivienda  
- **GrLivArea** (área habitable) presenta alta correlación positiva  
- La eliminación de outliers mejoró la estabilidad del modelo  
- La transformación logarítmica redujo el sesgo en la variable objetivo  

## Modelos Evaluados

| Modelo            | R²     | RMSE   |
|------------------|--------|--------|
| Regresión Lineal | 0.892  | 0.130  |
| Random Forest    | 0.858  | 0.149  |

## Decisión

La regresión lineal presentó mejor desempeño que Random Forest, lo que sugiere que las relaciones entre las variables son mayormente lineales en este conjunto de datos.

## Tecnologías

- Python  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- seaborn  

## Conclusión

El modelo logró explicar aproximadamente el 89% de la variabilidad del precio de las viviendas, demostrando que factores como la calidad general y el tamaño de la propiedad son determinantes clave en la predicción.
