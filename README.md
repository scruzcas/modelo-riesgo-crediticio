# Modelo de Clasificación de Riesgo Crediticio

Este proyecto fue desarrollado como parte de un reto de machine learning. El objetivo es construir un modelo de clasificación que identifique clientes riesgosos para una institución financiera, a partir de datos internos y externos.

## Archivos

- `notebook.ipynb`: Código completo del modelo, incluyendo limpieza de datos, feature engineering, entrenamiento con LightGBM y ajuste de hiperparámetros con Optuna.
- `presentacion.pdf`: Documento resumen con la justificación detallada de cada paso, resultados, conclusiones.

## Objetivo

Predecir la probabilidad de riesgo crediticio (variable objetivo `target`) con base en el comportamiento y características del cliente. Se utilizó la métrica AUC como principal criterio de evaluación.

## Resultados

- Modelo final: LightGBM con tuning por Optuna.
- AUC obtenido: aproximadamente 0.6043
- Se logró un alto recall para los clientes riesgosos ajustando el umbral de decisión.

## Herramientas utilizadas

- Python 3
- LightGBM
- Optuna
- Pandas, NumPy, Scikit-learn
- Matplotlib, Seaborn

## Notas

- Todas las gráficas en el notebook se encuentran incrustadas y no requieren volver a ejecutar celdas.
- Los datos fueron procesados localmente desde archivos `.parquet`.
