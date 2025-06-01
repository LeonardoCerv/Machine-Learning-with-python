
# Modelo de Análisis y Predicción de Gastos Personales

[![Language](https://img.shields.io/badge/code-Python-blue.svg?logo=python&logoColor=white)](https://python.org/)
[![Framework](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Colab](https://img.shields.io/badge/Google-Colab-orange.svg?logo=GoogleColab&logoColor=white)](https://scikit-learn.org/)
[![ML Library](https://img.shields.io/badge/Field-Machine%20Learning-red.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)

## Descripción del Proyecto

Este proyecto de ciencia de datos aborda la gestión de finanzas personales a través de modelado predictivo. Utilizando técnicas de aprendizaje automático, desarrollé un sistema que predice los costos de actividades basándose en múltiples variables incluyendo asignación presupuestaria, tipo de actividad, hora del día y número de participantes. El proyecto demuestra la aplicación práctica de la metodología CRISP-DM para resolver desafíos reales de planificación financiera.

**Planteamiento del Problema:** ¿Podemos predecir con precisión el costo de actividades personales basándonos en factores presupuestarios y contextuales, y usar estos conocimientos para mejorar la toma de decisiones financieras?

## Características Principales

- **Modelado Predictivo de Costos**: Modelo de regresión lineal que alcanza 85% de precisión (R² = 0.85)
- **Análisis Integral de Datos**: Análisis estadístico de 285+ registros de gastos a lo largo de 89 días
- **Perspectivas Financieras**: Cálculo automatizado de patrones de ahorro y recomendaciones de optimización presupuestaria
- **Visualización de Datos**: Comparaciones gráficas claras entre costos predichos y reales

## Implementación Técnica

### Tecnologías Utilizadas
- **Python**: Lenguaje de programación principal
- **Pandas**: Manipulación y análisis de datos
- **Scikit-learn**: Implementación de aprendizaje automático
- **Matplotlib**: Visualización de datos
- **Jupyter Notebooks**: Entorno de desarrollo interactivo
- **Google Colab**: Plataforma de ejecución basada en la nube

### Conceptos de Programación Aplicados

1. **Preprocesamiento y Validación de Datos**
   - Manejo sistemático de valores faltantes usando `dropna()` 
   - Validación de tipos de datos y estandarización de formato
   - Selección de características a través de subconjuntos de columnas (`iloc[:,3:9]`)

2. **Modelado Estadístico**
   - Implementación de regresión lineal con división entrenamiento-prueba (80/20)
   - Análisis de coeficientes para evaluación de importancia de características
   - Evaluación del modelo usando puntuación R² y análisis residual

3. **Manejo de Errores y Calidad de Datos**
   - Detección de valores nulos y procedimientos de limpieza
   - Verificaciones de integridad de datos antes y después del preprocesamiento
   - Refinamiento iterativo del modelo a través de múltiples ejecuciones

4. **Resolución Algorítmica de Problemas**
   - Ingeniería de características para variables categóricas (tipo de actividad, momento temporal)
   - Predicción multivariable usando presupuesto, tiempo, tipo, momento y tamaño del grupo
   - Cálculo de métricas financieras (tasa de ahorro, cronograma de logro de objetivos)

## Metodología: Marco CRISP-DM

### Fase 1: Comprensión del Negocio
- **Objetivo**: Predecir costos de actividades personales para mejorar la planificación presupuestaria
- **Criterios de Éxito**: Desarrollar un modelo que explique >80% de la varianza de costos
- **Interesado**: Optimización de gestión financiera personal

### Fase 2: Comprensión de los Datos
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QB_lH_D7s-Vi4gmNGMjiLfeD8VPEAWVw?usp=sharing)
- **Fuentes de Datos**: Registros de gastos personales (285 actividades, 89 días)
- **Variables Clave**: Presupuesto, Costo, Tipo de Actividad, Momento Temporal, Tamaño del Grupo
- **Calidad de Datos**: Identificación y tratamiento de valores faltantes en registros de costos

### Fase 3: Preparación de Datos  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1oP9cLpB8nw0WeR2r1aw2ijqvSLAy-brl?usp=sharing)
- **Selección de Datos**: Se enfocó en 6 atributos principales más relevantes para la predicción de costos
- **Limpieza**: Eliminación de registros con valores nulos para asegurar confiabilidad del modelo
- **Ingeniería de Características**: Preparación de variables categóricas para análisis de regresión
- **División de Entrenamiento**: 80% entrenamiento, 20% prueba para validación robusta

### Fase 4: Modelado de Datos
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jaAr7F8DuQHmI8Q75R8YxRFWM5c8gQR5?usp=sharing)
- **Algoritmo**: Regresión Lineal (implementación de scikit-learn)
- **Rendimiento**: R² = 0.85, indicando fuerte capacidad predictiva
- **Validación**: Análisis residual y comparación visual de costos predichos vs. reales
- **Iteración**: Tres intentos de modelado para optimizar parámetros y calidad de datos

## Resultados Clave

- **Precisión del Modelo**: 85% de la varianza de costos explicada por el modelo
- **Perspectivas Financieras**: 
  - Total de gastos rastreados: $71,630
  - Total de ahorros logrados: $17,830  
  - Ahorro diario promedio: $200
  - Logro de objetivo de lista de deseos: ~5 días para artículo de $1,000
- **Optimización Presupuestaria**: Identificación de patrones de actividades de alto costo para reducción dirigida

## Resultados de Aprendizaje Demostrados

**SEG0502 - Resolución de Problemas con Metodologías Válidas**: Aplicación sistemática del marco CRISP-DM para abordar un desafío real de gestión financiera, demostrando metodología rigurosa desde la comprensión del negocio hasta el despliegue.

**SEG0701 - Uso Estratégico de Tecnología Digital**: Aprovechamiento de Python, Jupyter notebooks y Google Colab para crear valor a través de conocimientos basados en datos, transformando datos de gastos brutos en inteligencia financiera accionable.

**SEG0702 - Evaluación e Implementación de Tecnología**: Evaluación de múltiples enfoques para preprocesamiento y modelado de datos, seleccionando regresión lineal basada en requisitos de interpretabilidad e implementando mejoras iterativas basadas en métricas de rendimiento.

## Reflexión Final

Este proyecto expandió significativamente mi comprensión de la ciencia de datos aplicada en finanzas personales, proporcionando experiencia práctica con el ciclo completo CRISP-DM desde la formulación del problema hasta conocimientos accionables. El aspecto más desafiante fue asegurar la calidad de los datos durante el preprocesamiento—identificar y manejar sistemáticamente valores faltantes me enseñó la importancia crítica de datos limpios en el éxito del aprendizaje automático.

La fase de modelado fue particularmente gratificante, permitiéndome presenciar cómo conceptos estadísticos abstractos se traducen en predicciones prácticas sobre comportamiento de gastos. Este trabajo fortaleció mis habilidades de programación en Python, especialmente en manipulación de datos con pandas y visualización con matplotlib, mientras me enseñó a pensar algorítmicamente sobre problemas del mundo real y validar soluciones a través de pruebas rigurosas.

Mirando hacia el futuro, planeo expandir este trabajo incorporando análisis de series temporales para patrones de gasto estacional y explorando métodos de conjunto para mejorar la precisión de predicción.
