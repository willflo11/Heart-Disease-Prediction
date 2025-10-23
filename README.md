# Proyecto: Predicción de Enfermedad Cardíaca

Este es un proyecto de Ciencia de Datos que utiliza Machine Learning para predecir la probabilidad de que un paciente tenga una enfermedad cardíaca, basado en un conjunto de datos clínicos del [repositorio UCI](https://archive.ics.uci.edu/ml/datasets/heart+Disease).

## Contexto y Objetivo

Como Médico General con especialización en enfermedades crónicas, mi objetivo era aplicar mis habilidades en Python y Data Science para construir un modelo de apoyo diagnóstico, enfocándome no solo en la precisión general, sino en la sensibilidad del modelo para evitar Falsos Negativos.

## Herramientas Utilizadas

* **Python**
* **Pandas:** Para la limpieza e imputación de datos.
* **Matplotlib / Seaborn:** Para el Análisis Exploratorio de Datos (EDA).
* **Scikit-learn:** Para el preprocesamiento (StandardScaler) y el modelado (Logistic Regression, Random Forest).

## Hallazgos Clave del EDA

* La edad y la frecuencia cardíaca máxima (`thalch`) mostraron una fuerte correlación con el diagnóstico.
* 
* Se encontró una correlación negativa contraintuitiva con el colesterol, probablemente debido a un sesgo de tratamiento (pacientes ya medicados).

## Resultados del Modelo

Se compararon dos modelos, siendo el **Random Forest** el ganador con un **Accuracy del 87%**.

Más importante aún, se optimizó el modelo para un escenario clínico, logrando una alta **Precisión (83%)** y **Sensibilidad (83%)**, minimizando así tanto los Falsos Positivos (costos innecesarios) como los Falsos Negativos (riesgo para el paciente).
