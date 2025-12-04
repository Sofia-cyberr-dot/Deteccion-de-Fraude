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