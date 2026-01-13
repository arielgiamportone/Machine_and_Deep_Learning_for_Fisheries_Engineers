# Datasets Sintéticos

Esta carpeta contiene datasets sintéticos creados para demostrar la aplicación de técnicas de Machine Learning y Deep Learning en el sector pesquero.

## Datasets Disponibles

### ✅ viabilidad_acuicultura.csv
**Descripción**: Datos ambientales y geográficos de sitios potenciales para acuicultura marina
- **Filas**: 40
- **Variables**: 9
- **Uso**: Clasificación binaria (viable/no viable)
- **Notebooks**: `ML_Supervisado_Clasificacion/Regresion_Log_Viabilidad_Proyecto_Acuicultura.ipynb`

**Variables**:
- `temperatura_C`: Temperatura del agua (°C)
- `salinidad_ppt`: Salinidad (partes por mil)
- `oxigeno_mg_L`: Oxígeno disuelto (mg/L)
- `pH`: Potencial de hidrógeno
- `profundidad_m`: Profundidad del sitio (metros)
- `distancia_costa_km`: Distancia a la costa (km)
- `exposicion_oleaje`: Exposición al oleaje (baja/media/alta)
- `tipo_fondo`: Tipo de sustrato (rocoso/arenoso/fangoso)
- `viable`: Variable objetivo (0=No viable, 1=Viable)

### ✅ desarrollo_larval_crustaceos.csv
**Descripción**: Datos de desarrollo larval de crustáceos decápodos en condiciones de cultivo
- **Filas**: 40
- **Variables**: 8
- **Uso**: Regresión (predicción de estadio larval)
- **Notebooks**: `ML_Supervisado_Regresion/RandomForest_Reg_estadio_larval.ipynb`

**Variables**:
- `temperatura_C`: Temperatura del agua (°C)
- `salinidad_ppt`: Salinidad (ppt)
- `pH`: Potencial de hidrógeno
- `oxigeno_mg_L`: Oxígeno disuelto (mg/L)
- `densidad_larvas_m3`: Densidad de cultivo (larvas/m³)
- `alimento_mg_dia`: Cantidad de alimento diario (mg/día)
- `dias_cultivo`: Días desde inicio del cultivo
- `estadio_larval`: Variable objetivo (1-5, Zoea I a Megalopa)

## Nota Importante

⚠️ **Estos datasets son sintéticos y creados con fines educativos**. No deben utilizarse para decisiones operativas reales. Para aplicaciones en producción, se recomienda:

1. Obtener datos reales de instituciones como:
   - INIDEP (Instituto Nacional de Investigación y Desarrollo Pesquero)
   - MAGYP (Ministerio de Agricultura, Ganadería y Pesca)
   - Centros de acuicultura y pesquerías locales

2. Validar modelos con expertos del sector

3. Realizar estudios de campo complementarios

## Contribuciones

Si tienes datasets reales que puedan ser compartidos (con las debidas autorizaciones y anonimizaciones), considera contribuir al proyecto. Ver [CONTRIBUTING.md](../CONTRIBUTING.md) para más información.

## Formato de Datos

Todos los datasets están en formato CSV con:
- Separador: coma (`,`)
- Encoding: UTF-8
- Primera fila: nombres de columnas
- Sin valores faltantes (para simplificar los ejemplos)

## Licencia de Datos

Los datasets sintéticos están bajo la misma licencia MIT del proyecto principal.
