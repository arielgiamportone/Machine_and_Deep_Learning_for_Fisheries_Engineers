# Guía de Contribución

¡Gracias por tu interés en contribuir a este proyecto! Esta guía te ayudará a empezar.

## Cómo Contribuir

### Reportar Bugs o Problemas

1. Verifica que el problema no haya sido reportado previamente
2. Abre un nuevo Issue describiendo:
   - Descripción clara del problema
   - Pasos para reproducirlo
   - Comportamiento esperado vs observado
   - Entorno (SO, versión de Python, etc.)

### Proponer Nuevas Características

1. Abre un Issue describiendo:
   - La característica propuesta
   - Justificación y casos de uso
   - Posible implementación

### Contribuir Código

#### 1. Fork y Clone

```bash
# Fork el repositorio en GitHub
# Luego clona tu fork
git clone https://github.com/tu-usuario/ML_DL_FisheriesEngineers.git
cd ML_DL_FisheriesEngineers
```

#### 2. Crear una Rama

```bash
git checkout -b feature/nueva-caracteristica
# o
git checkout -b fix/correccion-bug
```

#### 3. Realizar Cambios

- Sigue el estilo de código existente
- Documenta tus funciones y clases
- Agrega comentarios donde sea necesario
- Incluye docstrings en español

#### 4. Commit y Push

```bash
git add .
git commit -m "Descripción clara de los cambios"
git push origin feature/nueva-caracteristica
```

#### 5. Crear Pull Request

- Describe claramente los cambios
- Referencia Issues relacionados
- Asegúrate de que el código funcione correctamente

## Estándares de Código

### Python

- Sigue PEP 8
- Usa nombres descriptivos en español para variables específicas del dominio
- Mantén las funciones simples y enfocadas
- Longitud máxima de línea: 100 caracteres

### Notebooks

- Incluye markdown explicativo entre celdas de código
- Documenta cada sección claramente
- Incluye visualizaciones cuando sea apropiado
- Asegúrate de que todas las celdas se ejecuten en orden

### Estructura de Notebooks

```markdown
# Título del Notebook
## Objetivo
## Contexto
## 1. Carga de Datos
## 2. Análisis Exploratorio
## 3. Preprocesamiento
## 4. Modelado
## 5. Evaluación
## 6. Conclusiones
```

## Tipos de Contribuciones Bienvenidas

### 🔥 Altamente Valoradas

- **Notebooks completos** con nuevos casos de uso
- **Datasets reales** (con las debidas autorizaciones)
- **Correcciones de errores** en código o documentación
- **Mejoras en visualizaciones** y explicaciones
- **Traducciones** a otros idiomas
- **Casos de estudio** con datos del sector pesquero argentino

### ✅ También Valiosas

- Mejoras en el README
- Correcciones ortográficas
- Optimizaciones de código
- Nuevos ejemplos de uso
- Tests unitarios
- Documentación adicional

### 📚 Áreas Específicas

#### Notebooks por Implementar

- **ML_Supervisado_Clasificacion/**
  - Random Forest para procesamiento de productos
  - SVM para clasificación de capturas
  - KNN para identificación de buques eficientes
  - Naive Bayes para identificación de especies

- **ML_NoSupervisado_Clustering/**
  - PCA para análisis de flota
  - K-means para segmentación
  - DBSCAN para detección de patrones
  - Apriori para reglas de asociación

- **Deep_Learning_Imagenes_y_Sensores/**
  - CNNs para monitoreo satelital
  - Transfer learning para clasificación de especies
  - Segmentación de imágenes

- **Deep_Learning_SeriesTemporales/**
  - LSTMs para predicción de capturas
  - Análisis de series temporales oceanográficas

- **Deep_Learning_Causalidad_RedesBayesianas/**
  - Modelado de sostenibilidad pesquera
  - Análisis causal de ecosistemas

- **Deep_Learning_Grafos_y_Redes_Neuronales_Grafos/**
  - Optimización de cadenas de suministro
  - Análisis de redes de puertos

- **ML_Refuerzo/**
  - Políticas de cuotas de captura
  - Optimización de rutas de pesca

## Datasets

### Compartir Datos Reales

Si tienes acceso a datos reales del sector pesquero:

1. **Verifica permisos**: Asegúrate de tener autorización para compartir
2. **Anonimiza**: Remueve información sensible o privada
3. **Documenta**: Incluye metadatos completos
4. **Formato**: Preferiblemente CSV con encoding UTF-8
5. **Licencia**: Especifica la licencia de los datos

### Formato de Documentación de Datos

```markdown
## nombre_dataset.csv

**Fuente**: Institución/Fuente
**Período**: YYYY-MM a YYYY-MM
**Región**: Ubicación geográfica
**Variables**: N variables
**Filas**: N observaciones

### Variables:
- `variable1`: Descripción (unidad)
- `variable2`: Descripción (unidad)
...

### Notas:
- Notas relevantes sobre el dataset
```

## Código de Conducta

### Nuestro Compromiso

- Mantener un ambiente respetuoso e inclusivo
- Ser receptivos a feedback constructivo
- Enfocarse en lo que es mejor para la comunidad
- Mostrar empatía hacia otros miembros

### Comportamientos Esperados

✅ Uso de lenguaje acogedor e inclusivo
✅ Respeto a puntos de vista y experiencias diferentes
✅ Aceptación de críticas constructivas
✅ Enfoque en la colaboración

### Comportamientos Inaceptables

❌ Lenguaje o imágenes sexualizadas
❌ Comentarios insultantes o despectivos
❌ Acoso público o privado
❌ Publicar información privada sin permiso

## Proceso de Review

1. Todos los PRs serán revisados
2. Se pueden solicitar cambios
3. Una vez aprobado, se hará merge
4. Los contributors serán reconocidos

## Reconocimientos

Los contribuidores serán mencionados en:
- README principal
- Sección de agradecimientos
- Release notes cuando aplique

## Preguntas

Si tienes preguntas, puedes:
- Abrir un Issue con la etiqueta "pregunta"
- Contactar al mantenedor: giamportone1@gmail.com

---

**¡Gracias por contribuir al desarrollo de herramientas de ML/DL para el sector pesquero!** 🐟🤖
