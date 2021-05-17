---
layout: article
title: "Git me some credit"
categories: portfolio
excerpt: "Competición grupal de kaggle para predecir si en los próximos 2 años una persona puede pagar un crédito o no"
share: false
image:
  teaser: money-400x250.jpg
---

Los bancos juegan un papel crucial en las economías de mercado. Ellos deciden quién puede obtener financiamiento y en qué condiciones, y pueden tomar o deshacer decisiones de inversión. Para que los mercados y la sociedad funcionen, las personas y las empresas necesitan acceso al crédito.

Los algoritmos de calificación crediticia, que adivinan la probabilidad de incumplimiento, son el método que utilizan los bancos para determinar si se debe otorgar o no un préstamo. Esta competencia requiere que los participantes mejoren el estado del arte en la calificación crediticia, al predecir la probabilidad de que alguien experimente dificultades financieras en los próximos dos años.

El objetivo de esta competición era crear un modelo que los prestatarios pudieran utilizar para ayudar a tomar las mejores decisiones financieras.

Tras realizar previamente un análisis exploratorio de datos, informando las columnas que tenían algún dato sin valor con su media aritmética y representando la siguiente matriz de correlación para ver cómo de relacionadas estaban nuestras features (características) con el target(columna SeriousDlqin2yrs, valor que teníamos que predecir con nuestro modelo):

![image](https://github.com/sonimik13/portfolio/blob/gh-pages/images/matriz-750.jpg)


Una vez probados varios modelos, el modelo que mejor valores daba en entrenamiento era el modelo de clasificación de regresión logística binaria, con un AUC (área bajo la curva) de 0.73 y una predicción final con los datos de test de 0.69.

Para ver toda la documentación facilitada en la competición se puede acceder a la página web de [kaggle](https://www.kaggle.com/c/give-me-some-credit-20210326).

Todas las gráficas y el código del proyecto se pueden ver accediendo a este [repositorio](https://github.com/sonimik13/give-me-some-credit).
