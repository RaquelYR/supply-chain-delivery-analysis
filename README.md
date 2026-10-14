# Análisis de rendimiento en la cadena de suministro

El análisis completo se encuentra en [`docs/analisis.ipynb`](docs/analisis.ipynb).

## 1. Descripción del proyecto

Este proyecto analiza el rendimiento logístico de una cadena de suministro con el objetivo de identificar patrones asociados a los retrasos en las entregas y detectar oportunidades de mejora operativa.

El análisis se centra en comprender en qué situaciones se producen más retrasos, qué variables están relacionadas con una mayor probabilidad de entrega tardía y qué acciones podría priorizar la empresa para mejorar el cumplimiento de los plazos. Asimismo, se evalúa la capacidad de las variables disponibles para predecir retrasos mediante modelos de clasificación.

El proyecto consta de varias etapas: preparación y limpieza de los datos, análisis descriptivo, estudio de asociaciones entre variables y evaluación de modelos predictivos sencillos. Para las variables numéricas se utilizó correlación de Pearson y para las categóricas, V de Cramér. Finalmente, se probaron distintos modelos de machine learning para evaluar la capacidad predictiva de las variables disponibles.

## 2. Preguntas a responder

Durante el desarrollo del proyecto se trata de responder a las siguientes preguntas:

1. ¿Cuál es la tasa global de entregas tardías?
2. ¿Qué modos de envío presentan una mayor proporción de retrasos?
3. ¿Existen diferencias relevantes en el rendimiento logístico entre mercados, regiones o países de destino?
4. ¿Qué patrones temporales se observan en los retrasos?
5. ¿Qué variables están asociadas con una mayor probabilidad de entrega tardía?
6. ¿Hasta qué punto las variables disponibles permiten predecir el riesgo de retraso?
7. ¿Qué acciones podría priorizar la empresa para mejorar su rendimiento logístico?

## 3. Fuente de datos

Se utiliza el dataset "DataCo Smart Supply Chain for Big Data Analysis", disponible públicamente en Kaggle.

El conjunto de datos contiene información relacionada con pedidos, productos, clientes, mercados, métodos de envío, tiempos de entrega y riesgo de retraso, lo que permite analizar el rendimiento logístico desde diferentes perspectivas. 

Fuente: 

https://www.kaggle.com/datasets/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis

El dataset limpio preparado para el análisis exploratorio se incluye en la carpeta [`/data`](/data)

## 4. Herramientas

Para el desarrollo del proyecto se utilizan las siguientes herramientas: 

- **Python**:
    - Pandas y NumPy: preparación, limpieza, transformación y validación de los datos.
    - Matplotlib, Seaborn y Plotly: visualización de datos.
    - Scikit-learn: modelos de Machine Learning.
- **GitHub:** documentación y publicación final del proyecto.

## 5. Limitaciones

El dataset presenta una capacidad explicativa y predictiva limitada para estudiar los retrasos. Shipping Mode es la única variable con una asociación clara con Late_delivery_risk, mientras que el resto aporta poca información adicional. Faltan variables más relevantes para explicar las causas de los retrasos.

