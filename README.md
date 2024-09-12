# Evaluación de Machine Learning 🤖 

Este repositorio contiene la solución a cuatro problemas de Machine Learning, cada uno de ellos resuelto utilizando diferentes algoritmos y enfoques.
Los problemas varían desde la predicción del precio de viviendas hasta la detección de fraudes bancarios, pasando por la clasificación de correos spam y la recomendación de películas.

Cada problema se ha resuelto usando diferentes técnicas y algoritmos, y se presentan las métricas utilizadas para evaluar el rendimiento de los modelos.

# Problema 1️⃣: Predicción del Precio de Viviendas en California
Descripción:
Este problema busca predecir el precio de una casa en California basado en características como:
- Latitud
- Longitud
- Número de habitaciones
- Edad media de la casa
- Ingreso medio de los residentes

Dataset:
El dataset utilizado es [California Housing Prices](https://www.kaggle.com/datasets/camnugent/california-housing-prices).

Algoritmo Utilizado:
Se ha aplicado una Regresión Lineal para modelar la relación entre las características y el precio de la vivienda.

Métricas Utilizadas:
- Error Absoluto Medio (MAE): Mide el error promedio en las predicciones.
- Error Cuadrático Medio (MSE): Mide el error promedio al cuadrado en las predicciones, penalizando los errores grandes.
- R^2 (Coeficiente de determinación): Mide qué tan bien el modelo se ajusta a los datos.

Resultado:
El modelo de regresión lineal logra un R^2 razonable, lo que sugiere que las características tienen una relación clara con el precio de la vivienda. 
Las métricas de error muestran que el modelo tiene un desempeño aceptable, aunque podría beneficiarse de más ajustes o el uso de modelos más complejos.

-------------------------------------------------------------------------------------------------------------------------------------

# Problema 2️⃣: Clasificación de Correos Spam

Descripción:
Este problema busca clasificar correos electrónicos como **spam** o **no spam** basándose en el contenido del correo.

Dataset:
Se ha utilizado el dataset [Spambase](https://archive.ics.uci.edu/ml/datasets/Spambase), que contiene características de los correos, como la frecuencia de palabras y símbolos.

Algoritmo Utilizado:
Se ha implementado un **Random Forest Classifier**, un conjunto de árboles de decisión que mejora la precisión y evita el sobreajuste.

Métricas Utilizadas:
- Exactitud: Proporción de correos correctamente clasificados.
- Precisión: Proporción de correos predichos como spam que realmente lo son.
- Recall: Proporción de correos spam detectados por el modelo.
- F1-Score: Promedio armónico entre precisión y recall.

Resultado:
El modelo alcanza una alta exactitud y precisión, lo que significa que predice correctamente la mayoría de los correos spam sin clasificar erróneamente muchos correos legítimos como spam.
El recall es también aceptable, lo que indica que se detectan la mayoría de los correos spam.

---------------------------------------------------------------------------------------------------------------------------------------------

# Problema 3️⃣: Recomendación de Películas

 Descripción:
Este problema se enfoca en la recomendación de películas a un usuario basado en similitudes con otras películas o preferencias de otros usuarios.

 Dataset:
El dataset utilizado es [MovieLens 20M](https://www.kaggle.com/datasets/grouplens/movielens-20m-dataset), que contiene millones de calificaciones de películas por parte de usuarios.

 Algoritmo Utilizado:
Se ha utilizado un sistema de recomendación basado en la **Similitud del Coseno**, que mide qué tan similares son dos películas en función de sus calificaciones.

 Preguntas Resueltas:
- ¿Qué película recomendar si se quiere ver una película de terror?  
  Respuesta: El modelo recomienda películas que pertenecen al género de terror basándose en su popularidad.
  
- ¿Qué película recomendar si la última película fue Toy Story?
  Respuesta: El modelo identifica las películas más similares a Toy Story basándose en las calificaciones de los usuarios, recomendando películas con un perfil similar en cuanto a audiencia.

 Resultado:
El sistema de recomendación sugiere películas relevantes tanto por género como por similitud de calificaciones, utilizando las preferencias históricas de los usuarios para hacer recomendaciones 
personalizadas.

--------------------------------------------------------------------------------------------------------------------------------------------

# Problema 4️⃣: Detección de Fraude en Transacciones Bancarias

Descripción:
Este problema busca detectar si una transacción bancaria es fraudulenta o no, utilizando patrones históricos de transacciones.

Dataset:
El dataset utilizado es [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud), que contiene transacciones reales, donde algunas son fraudulentas y otras no.

Algoritmo Utilizado:
Se ha implementado un modelo de Support Vector Machine (SVM) con diferentes kernels (lineal, polinomial, RBF) para clasificar las transacciones como fraudulentas o no.

 Métricas Utilizadas:
- Exactitud: Proporción de transacciones correctamente clasificadas.
- Precisión: Proporción de transacciones predichas como fraudulentas que realmente lo son.
- Recall: Proporción de fraudes detectados por el modelo.
- F1-Score: Promedio armónico entre precisión y recall.

 Resultado:
El kernel RBF mostró el mejor rendimiento, con un balance adecuado entre precisión y recall, lo que permite detectar fraudes de manera eficiente sin clasificar erróneamente demasiadas 
transacciones legítimas como fraudulentas. El modelo tiene un F1-Score alto, lo que indica un buen equilibrio entre la detección de fraudes y la precisión.

----------------------------------------------------------------------------------------------------------------------------------------------------------

# Instrucciones de Uso
1. Clona el repositorio en tu máquina local.
2. Abre los notebooks (.ipynb) en Google Colab o un entorno Jupyter Notebook.
3. Ejecuta cada celda y sigue las instrucciones dentro de cada problema para entrenar y evaluar los modelos.
