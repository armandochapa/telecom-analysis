# telecom-analysis
Análisis de una empresa de telecomunicaciones

# 📱 Análisis de Comportamiento de Usuarios - ConnectaTel

🎯 Objetivo del Proyecto
Este proyecto analiza el comportamiento de uso de servicios móviles (llamadas y mensajes) de ConnectaTel, una empresa de telecomunicaciones con operaciones en México y Colombia.

### Objetivos específicos:
- Identificar patrones de uso de llamadas y mensajes por segmentos de clientes
- Detectar comportamientos atípicos que puedan indicar fraude o errores de registro
- Analizar cómo varía el uso según edad y tipo de plan contratado
- Generar insights comerciales para optimizar la oferta y mejorar la experiencia del usuario
- Crear segmentaciones de clientes basadas en comportamiento de uso y demografía

📊 Datasets Utilizados
El proyecto trabaja con tres fuentes principales de datos:

### 1. plans.csv
- Descripción: Catálogo de planes disponibles
- Contenido: Precio, minutos incluidos, GB incluidos, costo por servicios extra

### 2. users_latam.csv
- Descripción: Información demográfica y contractual de clientes
- Contenido: Edad, ciudad, país, fecha de registro, plan contratado, estado de churn

### 3. usage.csv
- Descripción: Registro detallado de actividad de usuarios
- Contenido: Duración de llamadas, cantidad de mensajes, longitud de mensajes

🔄 Etapas del Análisis Realizadas
### 1. Exploración y Carga de Datos
- Carga de los tres datasets
- Análisis inicial de estructura y dimensiones
- Identificación de tipos de datos

### 2. Limpieza y Preparación de Datos
- Detección y manejo de valores nulos
- Estandarización de tipos de datos
- Validación de consistencia entre datasets

### 3. Integración de Datos
- Unión de las tres fuentes de información
- Creación del dataset consolidado user_profile
- Validación de integridad de datos

### 4. Análisis Estadístico Descriptivo
- Estadísticas descriptivas de uso (llamadas y mensajes)
- Análisis de distribuciones por país y edad
- Identificación de patrones generales

### 5. Detección de Outliers
- Aplicación del método IQR (Rango Intercuartílico)
- Identificación de valores atípicos en:
  - Minutos de llamada
  - Cantidad de mensajes
  - Cantidad de llamadas

### 6. Segmentación de Clientes
- Segmentación por uso: Bajo uso, Uso medio, Alto uso
- Segmentación por edad: Joven (<30), Adulto (30-59), Adulto Mayor (60+)
- Análisis cruzado entre segmentos

### 7. Visualización y Análisis
- Gráficos de distribución por segmentos
- Validación visual de las segmentaciones creadas
- Identificación de insights comerciales

## 🚀 Cómo Ejecutar el Notebook

### Opción 1: Google Colab (Recomendado)
1. Abre [Google Colab](https://colab.research.google.com/)
2. Sube el archivo `connectatel_analysis.ipynb` (o el nombre de tu notebook)
3. Sube los archivos de datos (`plans.csv`, `users_latam.csv`, `usage.csv`) a la sección de archivos
4. Ejecuta las celdas secuencialmente desde el inicio

### Opción 2: Jupyter Notebook Local
1. Instala las dependencias necesarias:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
2. Clona o descarga este repositorio
3. Abre terminal en la carpeta del proyecto
4. Ejecuta: `jupyter notebook`
5. Abre el archivo `.ipynb` en el navegador

### Opción 3: Anaconda
1. Abre Anaconda Navigator
2. Lanza Jupyter Notebook
3. Navega hasta la carpeta del proyecto
4. Abre el archivo del notebook

## 📋 Guía de Reproducción

### Requisitos Previos
- **Python 3.7+**
- **Librerías necesarias**:
  - `pandas` (manipulación de datos)
  - `numpy` (cálculos numéricos)
  - `matplotlib` (visualizaciones básicas)
  - `seaborn` (visualizaciones estadísticas)

### Pasos para Reproducir el Análisis

1. **Preparación del Entorno**
   ```python
   import pandas as pd
   import numpy as np
   import matplotlib.pyplot as plt
   import seaborn as sns

2. **Carga de Datos**
- Asegúrate de que los archivos CSV estén en la misma carpeta que el notebook
- Ejecuta las celdas de carga de datos en orden

3. **Ejecución Secuencial**
- Importante: Ejecuta las celdas en orden secuencial
- No omitas ninguna celda de preparación de datos
- Verifica que cada paso se complete sin errores antes de continuar

4. **Validación de Resultados**
- Revisa que los datasets se carguen correctamente
- Verifica que las uniones de datos sean exitosas
- Confirma que las visualizaciones se generen apropiadamente
  
### Estructura de Archivos Esperada

proyecto_connectatel/

│

├── connectatel_analysis.ipynb

├── plans.csv

├── users_latam.csv

├── usage.csv

└── README.md

📈 Resultados Esperados
Al completar el análisis, obtendrás:
- Dataset consolidado con información completa de usuarios
- Identificación de outliers en patrones de uso
- Segmentaciones de clientes por uso y demografía
- Visualizaciones que validen los hallazgos
- Insights comerciales para estrategias de negocio

🤝 Contribuciones
Este proyecto forma parte del análisis de datos para telecomunicaciones. Para sugerencias o mejoras, por favor documenta tus hallazgos y propuestas de optimización.

---
Autor: Armando Chapa  
Fecha: 11-Feb-2026  
Versión: 1.0
```
