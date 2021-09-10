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

Para que los podemos usar? Para aumentar el engagement del público.

### Paquete Learnr

El paquete **{learnr}** en R nos permite hacer tutoriales interactivos de una manera muy fácil e intuitiva.

A continuación te presento algunas propuestas de uso de esta herramienta en el ambito de HR.

### Comunicaciones 

Acá por ejemplo, podemos hacer una pregunta abierta o solicitar sugerencias para "Regalos del día de..."

Las respuestas, con un poco de ayuda de código, las guardamos y luego analizamos.

*¿Qué te gustaría recibir para el día de....?*

```{r dos-mas-dos, exercise=TRUE}
# Escribilo entre " comillas "

```

### Juegos 

Juegos para públicos especificos. Por ejemplo un aviso para IT con un algoritmo en el que puedan encontrar el error o una lectura entre lineas de la info presentada.

```{r funcion-sumar-solution}
sumar <- function(numero1,numero2) {
  numero1+numero2
}

sumar(5,3)
```

### Preguntas 

Otra opción es incluir preguntas de opción única o múltiple.

Se usa la función `question` para definir una pregunta y la función`quiz` para agrupar varias preguntas.

Podemos usarlo para evaluar la gestión de una capácitación o en la evaluación de la entrevista por parte de un candidato.

```{r quiz_1}

quiz(
  question("¿Cómo podemos gestionar activamente la marca empleadora?", 
  correct = "Excelente! Son varios frentes para gestionar pero todos posibles.", 
  allow_retry = TRUE,
    answer("No hay presupuesto", message = "Otra vez será!"),
    answer("Pintando las salas", message = "Es bastante común!"),
    answer("Haciendo Reuniones", message = "Cuantas más mejor!."),
    answer("Pensando", correct = TRUE)
  ), caption = "Visualización"
)

```

Otra opción sería usar una serie de preguntas agrupadas con una o más de una respuesta correcta:

```{r quiz}
quiz(
  question("¿Tenemos una politica de diversidad?",
    answer("Si claro"),
    answer("No"),
    answer("Trababajamos en eso", correct = TRUE),
    answer("100% ")
  ),
  question("¿Es conveniente trabajar la diversidad en las organizaciones?",
    answer("Por supuesto ", correct = TRUE),
    answer("Depende"),
    answer("No"),
    answer(" Claro que si", correct = TRUE)
  )
)
```

### Conclusión

En este breve tutorial fuimos viendo algunas de las utilidades que podemos darle a esta herramienta desde RRHH.🚀

------------------------------------------------------------------------

[Yanel](https://yanelpaulette.netlify.app/)
