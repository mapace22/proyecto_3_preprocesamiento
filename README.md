# proyecto_3_preprocesamiento
Manipulación de datos (Data Wrangling) en streaming musical | Comparar preferencias y hábitos de escucha en 2 ciudades | Python | Pandas

# Análisis de Preferencias Musicales: Springfield vs. Shelbyville

## Resumen del Proyecto
Este proyecto de análisis de datos tiene como objetivo comparar las preferencias musicales de los habitantes de dos ciudades, Springfield y Shelbyville, utilizando datos reales de un servicio de streaming de música. A través de un enfoque estructurado, se explora el conjunto de datos para extraer información valiosa que pueda ser utilizada para la toma de decisiones estratégicas.

## Objetivo
La hipótesis principal a probar es la siguiente:

**"La actividad de los usuarios y las usuarias difiere según el día de la semana y dependiendo de la ciudad."**

## Metodología de Análisis
El proyecto se dividió en las siguientes etapas clave:

### 1. Descripción de los datos
- Inspección inicial del conjunto de datos
- Identificación del tipo de información disponible
- Revisión de la estructura de columnas
- Detección de problemas en la calidad de datos (valores ausentes, inconsistencias)

### 2. Preprocesamiento de datos
- **Estandarización de encabezados**:
  - Corrección de nombres de columnas
  - Estilo consistente (minúsculas, sin espacios, snake_case)
  
- **Manejo de valores ausentes**:
  - Identificación y reemplazo de valores NaN
  - Columnas afectadas: `track`, `artist` y `genre`
  - Reemplazo con el string `'unknown'`

- **Eliminación de duplicados**:
  - Tratamiento de duplicados explícitos (filas idénticas)
  - Unificación de duplicados implícitos (ej: hip, hop → hiphop)

### 3. Prueba de hipótesis
- Comparación del número total de canciones reproducidas por ciudad
- Análisis de actividad por días específicos (lunes, miércoles, viernes)
- Comparación de:
  - Volumen de reproducciones
  - Tendencias diarias
  - Diferencias entre ciudades

## Conclusiones Principales
Los resultados del análisis confirmaron la hipótesis inicial:

- **Disparidad de actividad**:
  - Springfield muestra mayor volumen de reproducciones que Shelbyville

- **Variación diaria**:
  - Picos de actividad: lunes y viernes
  - Descenso de actividad: mitad de semana

- **Confirmación de hipótesis**:
  - El consumo musical difiere entre ciudades
  - Varía significativamente según el día de la semana

## Tecnologías Utilizadas
- **Python** (lenguaje principal)
- **Pandas** (biblioteca para análisis y manipulación de datos)
