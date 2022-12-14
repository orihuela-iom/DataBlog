+++
author = "Orihuela I"
title = "Introducción a plotly"
date = "2022-08-11"
description = "En este primer articulo vamos a aprender a usar polty"
tags = [
    "markdown",
    "css",
    "html",
    "themes",
]
categories = [
    "Visualización",
    "Python",
]
series = ["Plotly-Dash"]
aliases = ["migrate-from-jekyl"]
plotly = true
image = "cover.png"
+++

<!--more-->

## Introducción a plotly
Plotly en una librería para visualización de datos, forma parte del proyecto Dash-Plotly el cual es un framework en python para elaborar dashboards, pero podemos hacer usos exclusivos de plotly para elaborar una gran variedad de graficas.
En este post nos enfocaremos en la versión de plotly para Python, aunque también está disponible en R o JavaScript o Julia.
Existen varias librerías populares para realizar gráficas, por mencionar algunas esta la clásica matlibplot, seaborn, altair la principal diferencia entra las antes mencionadas es que plotly permite elaborar gráficos interactivos lo que les dará un plus a tus visualizaciones. Aunque no es la única librería con estas capacidades, existe bokeh pero de ella hablaremos en otro post.

## Instalación.
Bien ahora sí a lo que venimos. Instalar plotly es muy sencillo y lo haremos por medio de consola y pip ejecutando el siguiente código:
```bash
pip install plotly==5.10.0
```

Ahora hablaremos un poco de como funciona, plotly trabaja de forma general con dos tipos de objetos: 
* graph_objects: Figuras tipo
* plotly.express: objetos de Plotly Express

El módulo graph_objects es el principal sobre el cual funciona plotly, nos permite un control total sobre todo los elementos de un gráfico con lo cual podremos personalizar a gusto nuestras visualizaciones, mientras que los objetos de plotly.express permite generar gráficas de manera rápida y con poco código, aunque está limitada en cuanto funcionalidad. Mi recomendación es usar siempre graph_objects.

## Usando plotly
Primero importaremos plotly mediante graph_objects y pandas para manipular algunos datos.
```python
import plotly.graph_objects as go
import  pandas as pd
```
Ahora creamos un dataframe con números aleatorios y crearemos un variable llamada fig donde primero declararemos un objeto tipo Figure y como argumento llamamos a la función go.Scatter() la cual nos servirá para crear una gráfica de línea:

```python
x = list(range(0,20))
y = np.random.randint(50, size=20)
fig = go.Figure(data=go.Scatter(x=x, y=y))
fig.show() 
```

{{< plotly json="/plots/hugo_plot.json" height="500px" >}}

Ahora creamos un dataframe con números aleatorios y crearemos un variable llamada fig donde primero declararemos un objeto tipo Figure y como argumento llamamos a la función go.Scatter() la cual nos servirá para crear una gráfica de línea:

## sin cambios
asjdnak sdaojsndkn  kasd kans d