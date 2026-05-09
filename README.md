# Análisis de Comportamiento Musical - "Déjame escuchar música"

## 📋 Descripción del Proyecto

Este proyecto analiza los patrones de comportamiento musical de usuarios en dos ciudades: **Springfield** y **Shelbyville**. El objetivo es determinar si existen diferencias significativas en los hábitos de escucha musical según la ubicación geográfica y el día de la semana.

## 🎯 Objetivos

- Comparar el comportamiento musical entre Springfield y Shelbyville
- Analizar patrones de escucha por día de la semana (lunes vs viernes)
- Identificar diferencias en diversidad de géneros musicales
- Evaluar la actividad de usuarios por ciudad y día

## 📊 Conjunto de Datos

**Archivo:** `music_project_en.csv`

**Estructura de datos:**

- **user_id**: Identificador único del usuario
- **track**: Título de la canción
- **artist**: Nombre del artista
- **genre**: Género musical
- **city**: Ciudad del usuario (Springfield/Shelbyville)
- **time**: Hora exacta de reproducción
- **day**: Día de la semana

**Volumen de datos:** 65,079 registros iniciales

## 🛠️ Tecnologías Utilizadas

- **Python 3.9+**
- **Pandas**: Manipulación y análisis de datos
- **Jupyter Notebook**: Entorno de desarrollo

## 📈 Principales Hallazgos

### Diferencias por Ciudad

- **Springfield**: 31,685 reproducciones totales
- **Shelbyville**: 11,509 reproducciones totales
- **Diferencia promedio**: 10,088 usuarios entre ciudades

### Diversidad Musical

- **Springfield**: 240 géneros únicos
- **Shelbyville**: 181 géneros únicos
- **Correlación**: Mayor población = mayor diversidad musical

### Patrones por Día

- **Viernes**: Ligeramente más activo que los lunes
- **Diferencia promedio**: 243 usuarios entre días
- **Tendencia**: Actividad similar entre lunes y viernes

## 🔧 Proceso de Limpieza de Datos

### Problemas Identificados y Solucionados:

**1. Estandarización de Columnas**

- Conversión a minúsculas
- Eliminación de espacios
- Aplicación de snake_case

**2. Valores Ausentes**

- **track**: 1,343 valores → reemplazados por 'unknown'
- **artist**: 7,567 valores → reemplazados por 'unknown'
- **genre**: 1,198 valores → reemplazados por 'unknown'

**3. Duplicados Explícitos**

- **Eliminados**: 3,826 registros duplicados

**4. Duplicados Implícitos**

- **Géneros unificados**: 'hip', 'hop', 'hip-hop' → 'hiphop'

## 📁 Estructura del Proyecto

```
proyecto-musica/
│
├── BP_project_template_ES_updated.ipynb    # Análisis principal
├── README.md                               # Este archivo
└── datasets/
    └── music_project_en.csv     
🚀 Cómo Ejecutar el Proyecto
Clonar el repositorio
git clone [url-del-repositorio]
cd proyecto-musica
Instalar dependencias
pip install pandas jupyter
Ejecutar el notebook
```bash
jupyter notebook BP_project_template_ES_updated.ip
