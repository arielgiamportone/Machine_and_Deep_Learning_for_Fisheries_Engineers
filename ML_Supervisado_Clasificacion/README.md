# Machine Learning Supervisado - Clasificación

Esta carpeta contiene notebooks que implementan algoritmos de clasificación supervisada aplicados a problemas del sector pesquero.

## Notebooks Disponibles

### ✅ Regresion_Log_Viabilidad_Proyecto_Acuicultura.ipynb
**Estado**: Implementado
- **Algoritmo**: Regresión Logística
- **Problema**: Clasificación de sitios para proyectos acuícolas
- **Dataset**: `../datasets/viabilidad_acuicultura.csv`
- **Objetivo**: Predecir si un sitio es viable para acuicultura marina basándose en variables ambientales

### 📋 Notebooks Planificados

- **Random_Forest_ProcesamientoProdPesq.ipynb**: Clasificación de calidad en procesamiento de productos pesqueros
- **SVM_Clas_captura.ipynb**: Clasificación de capturas en muestreos
- **KNN_buque_eficiente.ipynb**: Identificación de buques eficientes
- **Naive_Bayes_Identi_Especie.ipynb**: Identificación de especies comerciales

## Cómo Usar

1. Asegúrate de tener instaladas las dependencias:
```bash
pip install -r ../requirements.txt
```

2. Abre el notebook en Jupyter:
```bash
jupyter notebook Regresion_Log_Viabilidad_Proyecto_Acuicultura.ipynb
```

3. Ejecuta las celdas en orden para ver el análisis completo

## Conceptos Clave

- **Regresión Logística**: Modelo lineal para clasificación binaria
- **Random Forest**: Conjunto de árboles de decisión
- **SVM**: Clasificador de margen máximo
- **KNN**: Clasificación basada en vecinos más cercanos
- **Naive Bayes**: Clasificador probabilístico

## Métricas de Evaluación

- Accuracy (Exactitud)
- Precision (Precisión)
- Recall (Sensibilidad)
- F1-Score
- ROC-AUC
- Matriz de Confusión
