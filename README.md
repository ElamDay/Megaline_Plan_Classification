# Megaline Plan Classification

Proyecto de machine learning para clasificar clientes de Megaline entre los planes Smart y Ultra a partir de su comportamiento mensual.

## Objetivo

Desarrollar un modelo de clasificación con una exactitud mínima de 0.75 para recomendar uno de los nuevos planes de Megaline.

## Datos

El dataset contiene información mensual sobre:

- Número de llamadas
- Minutos totales
- Mensajes enviados
- Uso de Internet en MB
- Plan actual del cliente (`is_ultra`)

## Metodología

El proyecto incluye:

- Exploración inicial de los datos
- Separación de características y objetivo
- División en conjuntos de entrenamiento, validación y prueba
- Evaluación de árbol de decisión
- Evaluación de bosque aleatorio
- Evaluación de regresión logística
- Selección del mejor modelo
- Evaluación final en el conjunto de prueba
- Prueba de cordura con `DummyClassifier`

## Resultados

Los principales resultados fueron:

- Árbol de decisión: accuracy de validación ≈ 0.7854
- Random Forest: accuracy de validación ≈ 0.7916
- Regresión logística: accuracy de validación ≈ 0.7092
- Random Forest en el conjunto de prueba: accuracy ≈ 0.7932
- DummyClassifier: accuracy ≈ 0.6843

El modelo seleccionado fue Random Forest con `n_estimators=50`.

## Tecnologías utilizadas

- Python
- Pandas
- Scikit-learn
- Jupyter Notebook