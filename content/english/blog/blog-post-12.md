---
author: Yanel Paulette
bg_image: images/feature-bg.jpg
categories:
- Aplicación
date: "2021-09-01T11:07:10+06:00"
description: 
draft: false
image: images/blog/texto.png
tags:
- People Analytics
- blog
- Paquetes
- RRHH
title: Analizando textos 
type: post
---

## Analizando Textos

Desde RRHH trabajamos con personas, quienes interactuan, se comunican, y generan datos que circulan cada vez mas rapido. La mayoria de las veces, estos datos carecen de una estructura que pueda proporcionarnos utilidad. Acá es donde presentamos con aplausos a Text Mining👏👏.

¿ Qué es Text Mining, también llamado análisis de texto o mineria de datos? Consiste en la extracción de informacion interesante de un texto sin estructura, el cual no podriamos analizarlo a primera vista sin una intervencion técnica especifica. Para ello se desarrolla un proceso de fragmentación del texto, lo cual permite analizarlo y medir frecuencias de palabras, relaciones entre las mismas, incluso los sentimientos a los que puede evocar cada palabra.

Te invito a conocer el proceso para poder analizar los textos.

### Paquete Text Mining

El paquete **{Text Mining}** en R nos permite hacer analisis de textos.

Comparto un libro que me sirvio de guia para realizar mis proyectos. [Libro](https://www.tidytextmining.com/)

En RRHH analizar texto resulta fundamental, lo podriamos utilizar en entrevistas, evaluaciones, encuestas, comunicación corporativa, portales, redes sociales... mil usos que podriamos hacer según el objetivo buscado.

Pero sin maás presentaciones, vamos a hacer un ejemplo concreto del uso del paquete {**Text Mining**}

## Datos

Vamos a usar la base de datos de la [Encuesta de sueldos](https://rpubs.com/Data4HR/encuesta-kiwi-2020), que hicimos en el [Club de R para RRHH](https://rpubs.com/Data4HR/encuesta-kiwi-2020).

```{r}

library(DataExplorer)
library(googlesheets4)
library(tidyverse)
library(gargle)
library(tidytext)
library(wordcloud2)
library(tm)
library(funModeling)
library(scales)
library(gt)

# Estilos para los gráficos
zy <- theme(panel.background = element_blank(),
            panel.grid.major.y = element_line(colour = "#F4F6F6"),
            axis.line = element_line(colour = "grey"))

zx <- theme(panel.background = element_blank(),
            panel.grid.major.x = element_line(colour = "#F4F6F6"),
            axis.line = element_line(colour = "grey"))


# Cargar el archivo crudo

datos <- readRDS("kiwi_ar.RDS")

datos<- original

```

Lo primero que hacemos en conocer la estructura de nuestro dataset, lo cual  hacemos con la funcion str()

```{r}
str(datos)
limpios <- make.names(colnames(datos))
colnames(datos) <- limpios

rm(limpios)

```
Ahora quiero saber el tipo de dato que tengo


```{r}
datos2
```


Trabajar con datasets tan grandes, puede ser complejo, entonces voy a seleccionar solo aquellas variables con las que quiero trabajar para hacer el analisis de texto. 





## Conclusión

------------------------------------------------------------------------

[Yanel](https://yanelpaulette.netlify.app/)
