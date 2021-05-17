---
layout: article
title: "Estudio de la evolución del SARS-CoV-2 en España"
categories: portfolio
excerpt: "Análisis exploratorio de datos científicos desde el 01/01/2020 hasta el 09/03/2021 obtenidos del Instituto Carlos III"
share: false
image:
  teaser: covid-400x250.jpg
---

Me preocupaba y me preocupa el grado de afectación en la sociedad (hábitos, limitación de movilidad,..., y por encima de todo el número de fallecidos) tras la aparición del  
SARS-CoV-2 en nuestras vidas.

Esta preocupación es la que me ha llevado a realizar un estudio del SARS-CoV-2 en España para ver por qué situaciones habíamos pasado desde el inicio de la pandemia y 
dónde nos encontrábamos en el momento final del estudio, el 9 de marzo de 2021. No quería hacer cualquier tipo de estudio sino un estudio con rigor científico por lo que 
me he basado en los datos facilitados por el [Instituto Carlos III](https://cnecovid.isciii.es/covid19/).

En este proyecto EDA individual se ha analizado la incidencia del SARS-CoV-2 en cuanto a género y grupo de edad y se ha evaluado el impacto en cada CCAA (casos, 
hospitalizaciones, ingresos UCI, defunciones e IA a 14/7 días). 

La mayoría de los datos usados son cuantitativos por lo que se han realizado operaciones de `agrupación`, `conteo`, `sumatorio` y `ratios` concatenando o uniendo datasets 
en muchos de los casos.

Las conclusiones a las que se ha llegado tras realizar el estudio son las siguientes:

* En las mujeres es donde se han dado más casos de contagios (franja mayoritaria de contagios 40-49 años) aunque quienes más lo han sufrido han sido los hombres con 
un mayor número de hospitalizaciones, ingresos UCI y defunciones (en la franja total de 60-80 años)

* Las CCAA más castigadas en cuanto a número de defunciones teniendo en cuenta el índice de letalidad (número de defunciones/número de casos) serían Principado de Asturias,
Castilla-la Mancha, Castilla y León y Aragón

* Las CCAA más afectadas en cuanto a número de defunciones teniendo en cuenta el índice de mortalidad (número de defunciones por 100.000 habitantes) serían Castilla-la Mancha, 
Castilla y León, Aragón y La Rioja

* A fecha final de estudio, 9 de marzo de 2021, nos encontramos casi al final de la tercera ola en cada una de las CCAA (mayor IA a 14 días Melilla con 298,58 e IA a 7 días de
Melilla 119,43) 

En este proyecto se han desarrollado una gran variedad de visualizaciones gráficas, la mayor parte de ellas interactivas, utilizando las librerías `matplotlib`, `plotly`, `seaborn` y `folium`. 

A continuación se muestra una de las gráficas generadas:
