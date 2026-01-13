# Machine Learning Supervisado - Regresión

Esta carpeta contiene notebooks que implementan algoritmos de regresión supervisada para predecir valores continuos en contextos pesqueros.

## Notebooks Disponibles

### ✅ RandomForest_Reg_estadio_larval.ipynb
**Estado**: Implementado
- **Algoritmo**: Random Forest Regressor
- **Problema**: Predicción de estadio de desarrollo larval en crustáceos
- **Dataset**: `../datasets/desarrollo_larval_crustaceos.csv`
- **Objetivo**: Predecir el estadio larval basándose en variables ambientales y de cultivo

### 📋 Notebooks Planificados

- **SVM_Salmones.ipynb**: Modelado de crecimiento en salmónidos en sistemas RAS
- **LinearRegression_Biomasa.ipynb**: Estimación de biomasa en pesquerías
- **XGBoost_Produccion.ipynb**: Predicción de producción en acuicultura

## Cómo Usar

1. Instala las dependencias:
```bash
pip install -r ../requirements.txt
```

2. Abre el notebook:
```bash
jupyter notebook RandomForest_Reg_estadio_larval.ipynb
```

3. Ejecuta las celdas secuencialmente

## Conceptos Clave

- **Regresión Lineal**: Relación lineal entre variables
- **Random Forest Regressor**: Ensemble de árboles para regresión
- **Support Vector Regression (SVR)**: Regresión con vectores de soporte
- **Gradient Boosting**: Modelos de boosting para regresión

## Métricas de Evaluación

- R² (Coeficiente de Determinación)
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- MAPE (Mean Absolute Percentage Error)
- Validación Cruzada

## Casos de Uso

- Predicción de crecimiento de especies cultivadas
- Estimación de biomasa
- Modelado de rendimiento productivo
- Predicción de parámetros de calidad del agua
