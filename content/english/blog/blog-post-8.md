---
title: "Tutorial Interactivo para HR"
output:
  learnr::tutorial:
    progressive: true
    allow_skip: true
runtime: shiny_prerendered
description: "Paquete Learnr"
---

```{r setup, include=FALSE}
library(learnr)
knitr::opts_chunk$set(echo = FALSE)
```


## Intro

Esta semana descubrí un paquete en R {learnr} con el cual se pueden hacer tutoriales interactivos como el presente. 

Ustedes se preguntarán...¿En RRHH...?  👇

![](https://media.giphy.com/media/kFVtWU2FLQqVilrIT1/giphy.gif)

Te invito a que pensemos juntos Cómo podriamos aplicarlo en HR?🚀 



## Comunicaciones 📪

Acá por ejemplo, podemos  hacer  una pregunta abierta o solicitar  sugerencias para "Regalos del día de..." 

Las respuestas, con un poco de ayuda de código, las guardamos  y luego analizamos.

*¿Qué te gustaría recibir para el día de....?* ✨


```{r dos-mas-dos, exercise=TRUE}
# Escribilo entre " comillas "

```

## Juegos 🎯 

Juegos para públicos especificos. Por ejemplo un aviso para IT  con un algoritmo en el que  puedan encontrar el error o una lectura entre lineas de la info presentada.


```{r funcion-sumar, exercise=TRUE, exercise.lines = 5}
sumar <- function(___,___) {
  ______
}

sumar(___,___)
```

```{r funcion-sumar-hint}
sumar <- function(___,___) {
  # Aqui debe ir el calculo sumando los dos parámetros 
  # que debe tener la función para recibir los dos números a sumar
}

sumar(___,___)
```

```{r funcion-sumar-solution}
sumar <- function(numero1,numero2) {
  numero1+numero2
}

sumar(5,3)
```


## Preguntas ❓


Otra opción es incluir preguntas  de opción única o múltiple.

Se usa la función `question` para definir una pregunta y la función` quiz` para agrupar varias preguntas.

Podemos usarlo para evaluar la gestión de una capácitación  o en la evaluación de la entrevista por parte de un candidato.


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

Otra opción sería usar una  serie de preguntas agrupadas con una o   más de una respuesta correcta:

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

## Fin 

En este breve tutorial fuimos viendo algunas de  las utilidades  que podemos darle a esta herramienta desde RRHH. 


Se te ocurren otras? Compartilo en comentarios! 👇 


--------------------------

[Yanel Paulette](https://www.linkedin.com/in/yanelpaulette/)

Contacto: <http://linktr.ee/Yanel.Paulette/>


-------------------------
Gracias a [Yanina Saibene](https://learning-learnr.netlify.app/courses/textmining/) por compartir el tutorial. 

