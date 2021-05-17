---
layout: article
title: "NPL en la red social Twitter"
categories: portfolio
excerpt: "Competición grupal de kaggle para predecir si un tweet está hablando de un desastre o no"
share: false
image:
  teaser: twitter-400x250.jpg
---

A partir de una serie de tweets había que crear un modelo de predicción para clasificar si el tweet estaba hablando de un desastre o no. 

Nuestro dataset de entrenamiento constaba de la target (valor que teníamos que predecir con nuestro modelo) y las siguientes 4 features (características):

- id: identificador del tweet 
- keyword: palabra clave del tweet 
- location: localización del tweet 
- text: el texto del tweet 

Se han descartado los datos id, location y keyword para realizar la predicción del modelo ya que nuestro modelo lo que tenía que hacer es, en función de los datos contenidos en text, predecir si se estaba hablando de un desastre o no.

Como pretratamiento se ha realizado una limpieza de datos en la columna text que ha consistido en lo siguiente: pasar todas las letras del texto a minúsculas,
eliminar caracteres especiales (@, #,\,...) y eliminar las stop words o palabras vacías (artículos, preposiciones, sujetos,...)

Un siguiente paso común en el preprocesamiento de texto es normalizar las palabras de su corpus tratando de convertir todas las diferentes formas de una palabra dada en una sola. Dos métodos que existen para esto son Stemming y Lemmatization.

En este caso se ha usado el método Lemmatization que consiste en transformar la palabra en su verdadera raíz y mediante la búsqueda de la mejor combinación de hiperparámetros posible usando la transformación TF-IDF (que es la representación del número de veces que una palabra determinada aparece en un documento en relación con el número de documentos en el corpus en el que aparece la palabra donde las palabras que aparecen en muchos documentos tienen un valor más cercano a cero y las palabras que aparecen en menos documentos tienen valores más cercanos a 1) y el algoritmo de SVM, consiguiendo un valor de AUC (área bajo la curva) en entrenamiento de 0.72 y una predicción final con los datos de test de 0.83.

Para ver toda la documentación facilitada en la competición se puede acceder a la página web de [kaggle](https://www.kaggle.com/c/the-bridge-nlp/overview).

Todo el código del proyecto se puede ver accediendo a este [repositorio](https://github.com/sonimik13/NLP-en-la-red-social-Twitter).
