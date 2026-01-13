# Guía de Instalación Detallada

Esta guía proporciona instrucciones paso a paso para configurar el entorno de desarrollo.

## Requisitos del Sistema

### Hardware Recomendado
- **CPU**: Procesador de 4 núcleos o superior
- **RAM**: Mínimo 8 GB (recomendado 16 GB para Deep Learning)
- **Almacenamiento**: 5 GB de espacio libre
- **GPU** (opcional): Para entrenar modelos de Deep Learning más rápido

### Software Necesario
- **Sistema Operativo**: Windows 10/11, macOS, o Linux
- **Python**: Versión 3.8 o superior
- **Git**: Para clonar el repositorio

## Instalación Paso a Paso

### 1. Instalar Python

#### Windows
1. Descargar desde [python.org](https://www.python.org/downloads/)
2. Ejecutar el instalador
3. ✅ Marcar "Add Python to PATH"
4. Verificar instalación:
```bash
python --version
pip --version
```

#### macOS
```bash
# Con Homebrew
brew install python@3.11

# Verificar
python3 --version
pip3 --version
```

#### Linux (Ubuntu/Debian)
```bash
sudo apt update
sudo apt install python3 python3-pip

# Verificar
python3 --version
pip3 --version
```

### 2. Instalar Git

#### Windows
Descargar desde [git-scm.com](https://git-scm.com/download/win)

#### macOS
```bash
brew install git
```

#### Linux
```bash
sudo apt install git
```

### 3. Clonar el Repositorio

```bash
# Navegar a la carpeta donde quieres el proyecto
cd ~/Documentos  # o la ruta que prefieras

# Clonar
git clone https://github.com/PesquerosEnIA/ML_DL_FisheriesEngineers.git

# Entrar al directorio
cd ML_DL_FisheriesEngineers
```

### 4. Crear Entorno Virtual (Recomendado)

#### ¿Por qué usar un entorno virtual?
- Aísla las dependencias del proyecto
- Evita conflictos con otros proyectos
- Facilita la reproducibilidad

#### Crear entorno virtual

**Windows:**
```bash
# Crear entorno virtual
python -m venv venv

# Activar
venv\Scripts\activate
```

**macOS/Linux:**
```bash
# Crear entorno virtual
python3 -m venv venv

# Activar
source venv/bin/activate
```

Cuando esté activado, verás `(venv)` al inicio de la línea de comandos.

### 5. Instalar Dependencias

```bash
# Asegúrate de que el entorno virtual esté activado
# Deberías ver (venv) en la terminal

# Actualizar pip
python -m pip install --upgrade pip

# Instalar todas las dependencias
pip install -r requirements.txt
```

⏱️ **Tiempo estimado**: 5-15 minutos (depende de tu conexión a internet)

### 6. Verificar Instalación

```python
# Crear un archivo test_install.py
import sys
print(f"Python: {sys.version}")

import numpy as np
print(f"NumPy: {np.__version__}")

import pandas as pd
print(f"Pandas: {pd.__version__}")

import sklearn
print(f"Scikit-learn: {sklearn.__version__}")

import tensorflow as tf
print(f"TensorFlow: {tf.__version__}")

print("\n✅ Todas las bibliotecas principales están instaladas correctamente!")
```

Ejecutar:
```bash
python test_install.py
```

### 7. Iniciar Jupyter Notebook

```bash
jupyter notebook
```

Esto abrirá tu navegador con la interfaz de Jupyter. Navega a cualquier `.ipynb` para empezar.

## Solución de Problemas Comunes

### Error: "Python no se reconoce como comando"
**Solución**: Agrega Python al PATH del sistema
- Windows: Reinstalar Python marcando "Add Python to PATH"
- macOS/Linux: Usar `python3` en lugar de `python`

### Error al instalar TensorFlow
**Solución para Windows**:
```bash
# Instalar versión compatible con CPU
pip install tensorflow-cpu
```

**Solución para macOS con Apple Silicon (M1/M2)**:
```bash
# Usar versión optimizada para Metal
pip install tensorflow-macos
pip install tensorflow-metal
```

### Error: "No module named 'xyz'"
**Solución**:
```bash
# Reinstalar la dependencia específica
pip install xyz

# O reinstalar todas
pip install -r requirements.txt --force-reinstall
```

### Jupyter no se abre
**Solución**:
```bash
# Reinstalar Jupyter
pip uninstall jupyter notebook
pip install jupyter notebook

# Iniciar en un puerto diferente
jupyter notebook --port 8889
```

### Error de memoria al entrenar modelos
**Solución**:
- Reducir tamaño de batch
- Usar menos datos para pruebas
- Cerrar otros programas
- Considerar usar Google Colab (gratis con GPU)

## Instalación en Google Colab (Alternativa)

Si tienes problemas con la instalación local, puedes usar Google Colab:

1. Ve a [colab.research.google.com](https://colab.research.google.com)
2. Carga un notebook desde GitHub:
   - File → Open notebook → GitHub tab
   - URL: `https://github.com/PesquerosEnIA/ML_DL_FisheriesEngineers`
3. Las dependencias principales ya están instaladas
4. Para dependencias adicionales:
```python
!pip install pgmpy torch-geometric
```

## Actualizar el Proyecto

Para obtener las últimas actualizaciones:

```bash
# Navegar al directorio del proyecto
cd ML_DL_FisheriesEngineers

# Obtener cambios
git pull origin main

# Actualizar dependencias (si hay cambios en requirements.txt)
pip install -r requirements.txt --upgrade
```

## Desactivar Entorno Virtual

Cuando termines de trabajar:

```bash
deactivate
```

## Desinstalar

Para eliminar completamente el proyecto:

```bash
# Navegar al directorio padre
cd ..

# Eliminar carpeta del proyecto
rm -rf ML_DL_FisheriesEngineers  # Linux/macOS
# o
rmdir /s ML_DL_FisheriesEngineers  # Windows

# Eliminar entorno virtual si lo creaste
rm -rf venv  # Linux/macOS
rmdir /s venv  # Windows
```

## Recursos Adicionales

### Tutoriales de Python
- [Python.org Tutorial](https://docs.python.org/3/tutorial/)
- [Real Python](https://realpython.com/)

### Tutoriales de Jupyter
- [Jupyter Documentation](https://jupyter-notebook.readthedocs.io/)
- [Dataquest Jupyter Tutorial](https://www.dataquest.io/blog/jupyter-notebook-tutorial/)

### Tutoriales de Git
- [Git Handbook](https://guides.github.com/introduction/git-handbook/)
- [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials)

## Soporte

Si encuentras problemas no cubiertos aquí:

1. Revisa los [Issues](https://github.com/PesquerosEnIA/ML_DL_FisheriesEngineers/issues) del proyecto
2. Abre un nuevo Issue describiendo tu problema
3. Contacta: giamportone1@gmail.com

---

**¡Listo para empezar!** 🚀

Una vez instalado todo, comienza con:
```bash
jupyter notebook ML_and_DL_for_FisheriesEngineers.ipynb
```
