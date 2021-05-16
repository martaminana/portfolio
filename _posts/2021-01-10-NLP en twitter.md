---
layout: article
title: "NPL en la red social Twitter"
categories: portfolio
excerpt: "Competición grupal de kaggle para predecir si un tweet está hablando de un desastre o no"
share: false
image:
  teaser: twitter-400x250.jpg
---

A partir de una serie de tweets se ha creado un modelo de predicción para clasificar si el tweet estaba hablando de un desastre o no.

Nuestro dataset tenía 4 features más la target.

- id: identificador del tweet 
- keyword: palabra clave del tweet 
- location: localización del tweet 
- text: el texto del tweet 

Se han descartado los datos id, location y keyword para realizar la predicción del modelo.

Como pretratamiento se ha realizado una limpieza de datos en la columna text que ha consistido en lo siguiente: pasar todas las letras del texto a minúsculas,
eliminar caracteres especiales (@, #,\,...) y eliminar las stop words o palabras vacías (artículos, preposiciones, sujetos,...)

Un siguiente paso común en el preprocesamiento de texto es normalizar las palabras de su corpus tratando de convertir todas las diferentes formas de una palabra dada en una sola. Dos métodos que existen para esto son Stemming y Lemmatization.

En este caso se ha usado el método Lemmatization que consiste en transformar la palabra en su verdadera raíz y mediante la búsqueda de la mejor combinación de hiperparámetros posible usando   
la transformación TF-IDF (que es la representación del número de veces que una palabra determinada aparece en un documento en relación con el número de documentos en el corpus en el que aparece la palabra
donde las palabras que aparecen en muchos documentos tienen un valor más cercano a cero y las palabras que aparecen en menos documentos tienen valores más cercanos a 1) y el algoritmo de SVM, se ha
conseguido un valor de AUC (área bajo al curva) de 0.72.

Todas las gráficas y el código del proyecto se pueden ver accediendo a este [repositorio](https://github.com/sonimik13/NLP-en-la-red-social-Twitter).
