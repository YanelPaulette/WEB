---
author: Yanel Paulette
bg_image: images/feature-bg.jpg
categories:
- Presentación
date: "2021-07-19T11:07:10+06:00"
description: 
draft: false
image: images/blog/engagement.jpg
tags:
- People Analytics
- blog
- Paquetes
- RRHH
title: Tutoriales 
type: post
---

## Tutoriales Interactivos

Los tutoriales interactivos son una herramientas que permiten la interacción con el usuario a partir de una experiencia inmersiva.

¿Para qué los podemos usar? Para aumentar el engagement del público 🤩

A continuación te cuento una breve introduccion. Ingresando a la siguiente publicación podes probar la herramienta, la cual hice con otro paquete de R { [Shiny](https://shiny.rstudio.com/)} que facilita la creación de aplicaciones web interactivas. 💻 [Tutorial](https://yanelpaulette.shinyapps.io/Tutorial_Interactivo/)

### Paquete Learnr

El paquete **{[learnr](https://rstudio.github.io/learnr/)}** en R nos permite hacer tutoriales interactivos de una manera muy fácil e intuitiva.

A continuación te presento algunas propuestas de uso de esta herramienta en el ambito de HR.

### Comunicaciones 

Podemos hacer una pregunta abierta o solicitar sugerencias para "Regalos del día de..."

Las respuestas, con un poco de ayuda de código, las guardamos y luego analizamos.

*¿Qué te gustaría recibir para el día de....?*

```{r dos-mas-dos, exercise=TRUE}
# solicitamos al usuario escriba sus propuestas

```

### Preguntas 

Otra opción es incluir preguntas de opción única o múltiple.

Se usa la función `question` para definir una pregunta y la función`quiz` para agrupar varias preguntas.

Podemos usarlo para evaluar la gestión de una capácitación o en la evaluación de la entrevista por parte de un candidato.

![](/images/blog/preg1.JPG)

Otra opción sería usar una serie de preguntas agrupadas con una o más de una respuesta correcta:

![](/images/blog/preg2.JPG)

![](/images/blog/preg3.JPG)

## Conclusión

En este breve tutorial fuimos viendo algunas de las utilidades que podemos darle a este paquete desde RRHH.🚀

------------------------------------------------------------------------

[Yanel](https://yanelpaulette.netlify.app/)
