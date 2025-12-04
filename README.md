# Proyecto de Deteccion de Fraude

Sistema Simulado de Detección de Fraude en Transacciones Bancarias



# 1. Descripción General del Proyecto

Este proyecto simula un sistema de detección de fraude bancario utilizando técnicas de Machine Learning.
Se crea un dataset sintético y se entrena un modelo capaz de identificar patrones sospechosos en las transacciones, ayudando a reducir pérdidas y mejorar la seguridad financiera.

El objetivo es mostrar un flujo de trabajo profesional que incluya:

preparación de datos, análisis exploratorio,
entrenamiento del modelo,evaluación,documentación del proyecto.

# 2. Dataset Utilizado

El dataset utilizado es sintético, creado especialmente para este proyecto, con 10.000 transacciones ficticias.

Campos incluidos:

monto
pais
tipo_transaccion
hora
dispositivo
fraud_flag (0 = legítima, 1 = fraude)
El archivo se encuentra dentro de:
/data/fraude.csv

# 3. Objetivo del Modelo

El objetivo principal es predecir si una transacción bancaria es fraudulenta utilizando un modelo de clasificación supervisada.

Algoritmos utilizados o sugeridos:

Regresión Logística
Árboles de Decisión
Random Forest
Redes Neuronales (opcional)

#  4. Metodología Ágil — Mini Sprint Planning
 Sprint 1 — Preparación del entorno
Crear repositorio GitHub
Crear carpetas /src, /data, /notebooks
Generar dataset sintético
Instalar dependencias

 Sprint 2 — Procesamiento y Análisis de Datos
Cargar dataset
Limpieza básica
Análisis exploratorio
Visualización de métricas y outliers

 Sprint 3 — Entrenamiento del Modelo
División Train/Test
Pruebas con diferentes modelos
Selección del mejor algoritmo

 Sprint 4 — Evaluación y Documentación
Matriz de confusión
Accuracy, Precision, Recall, F1
Comentarios finales
Completar README.md

# 5. Herramientas y Tecnologías Utilizadas

Python 3.10+
Pandas
NumPy
Scikit-learn
Matplotlib / Seaborn
Jupyter Notebook
VS Code
Git
GitHub
Trello (metodología ágil)

![Tabla de promedios](./img/tabla_promedios.png)



# Ejecución y Desarrollo (Flujo de Trabajo Detallado)

Esta sección describe el proceso de trabajo realizado en cada etapa, cumpliendo con los criterios de Ejecución y Herramientas.

6.1. Preprocesamiento de Datos (Sprint 2)
Carga y Limpieza: Se cargó el archivo fraude.csv. Se verificaron valores nulos y tipos de datos.

Análisis Exploratorio de Datos (EDA): Se analizaron las distribuciones de monto, hora y la proporción de transacciones fraudulentas vs. legítimas (se encontró un desbalance de clases).

Ingeniería de Características: Se aplicó One-Hot Encoding a las variables categóricas (pais, tipo_transaccion, dispositivo). Se normalizó/escaló la variable monto.

6.2. Entrenamiento y Selección del Modelo (Sprint 3)
División Train/Test: Los datos se dividieron en conjuntos de entrenamiento y prueba (e.g., 70/30).

Manejo del Desbalance: Dada la baja proporción de fraudes, se aplicó una técnica de sobremuestreo (e.g., SMOTE) o se ajustó la ponderación de clases (class weights).
Pruebas Iniciales: Se entrenaron y compararon la Regresión Logística y los Árboles de Decisión.
Modelo Final: Se seleccionó Random Forest por su robustez y mejor rendimiento en las métricas de Recall y F1-Score.




#  Reproducción del Proyecto
Para replicar este proyecto en tu entorno local, sigue los siguientes pasos:

8.1. Estructura del Repositorio

![estructura repositorio](./img/pi.png)


8.2. Instalación de Dependencias
Clona el repositorio:

Bash
![clona el repositorio](./img/pu.png)


Instala las librerías necesarias:

Bash

pip install -r requirements.txt
Archivo requirements.txt (Ejemplo de contenido):

![librerias](./img/pe.png)

8.3. Ejecución
Abre el entorno Jupyter/VS Code.

Ejecuta secuencialmente los notebooks ubicados en /notebooks para ver el flujo de trabajo completo, desde la carga de datos hasta la evaluación final del modelo.

#  9. Conclusiones y Aprendizajes (Comentarios Finales)


A lo largo del desarrollo de este proyecto, se fortalecieron significativamente los aprendizajes técnicos, adquiriendo experiencia práctica en el manejo de librerías de Python, análisis de datos y desarrollo de modelos de detección de fraude. Además, se potenciaron las habilidades profesionales, tales como la organización del trabajo, la resolución de problemas y la capacidad de documentar y presentar resultados de manera clara. Finalmente, se identificaron mejoras futuras, como optimizar el rendimiento de los modelos, explorar nuevas técnicas de análisis y ampliar la cobertura de datos para obtener resultados más precisos y robustos. Este proyecto no solo consolidó conocimientos adquiridos, sino que también sentó las bases para continuar creciendo y perfeccionando las competencias tanto técnicas como profesionales.