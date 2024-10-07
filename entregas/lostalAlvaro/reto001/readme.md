# Reto 001 / Ejercicio 3

## Introducción

Con lo visto en clase, he desarrollado 4 diagramas UML que representan dos conceptos: **el eco** y **la toma de decisiones**. Para cada concepto, he elaborado un diagrama de clases y un diagrama de objetos, respetando las estructuras requeridas.

## Eco

### Diagramas

| Nombre                      | Imagen                                                         |
|-----------------------------|----------------------------------------------------------------|
| Diagrama de clases de Eco   | ![Diagrama de Clases Eco](/entregas/lostalAlvaro/reto001/img/EcoClases.svg)             |
| Diagrama de objetos de Eco  | ![Diagrama de Objetos Eco](/entregas/lostalAlvaro/reto001/img/EcoObjetos.svg)           |

### Explicación

- **Diagrama de clases de Eco**: Este diagrama representa las clases **Sonido**, **Vibraciones**, **Barrera** y **Eco**. La clase **Sonido** genera **Vibraciones**, las cuales se reflejan en una **Barrera** para producir el **Eco**. Además, el **Eco** influye en el **Sonido**, estableciendo una relación de retroalimentación.

- **Diagrama de objetos de Eco**: Este diagrama muestra instancias específicas como **Grito**, **VibracionesGrito**, **Pared** y **EcoGrito**. El **Grito** genera **VibracionesGrito**, que se reflejan en una **Pared** produciendo **EcoGrito**. El **EcoGrito** influye nuevamente en el **Grito**, demostrando una interacción concreta del fenómeno.

## Toma De Decisiones

### Diagramas

| Nombre                      | Imagen                                                         |
|-----------------------------|----------------------------------------------------------------|
| Diagrama de clases de Toma de Decisiones   | ![Diagrama de Clases Eco](/entregas/lostalAlvaro/reto001/img/TomaDeDecisionesClases.svg)             |
| Diagrama de objetos de Toma de Decisiones  | ![Diagrama de Objetos Eco](/entregas/lostalAlvaro/reto001/img/TomaDeDecisionesObjetos.svg)           |

### Explicación

- **Diagrama de clases de Toma de Decisiones**: Este diagrama incluye las clases **Decisor**, **Conflicto**, **Idea**, **Analisis** y **Decision**. El **Decisor** enfrenta un **Conflicto** que deriva en una **Idea**. La **Idea** es evaluada por un **Analisis**, que puede rechazarla si no es válida o proceder a una **Decision** si es aceptada. La **Decision** impacta al **Decisor**, cerrando el ciclo del proceso decisorio.

- **Diagrama de objetos de Toma de Decisiones**: En este diagrama se observan instancias específicas como **Persona**, **Dilema**, **IdeaSolucion**, **AnalisisSolucion** y **Eleccion**. La **Persona** enfrenta un **Dilema** que genera una **IdeaSolucion**. Esta idea es revisada por un **AnalisisSolucion**, que puede rechazarla si es incorrecta o aceptar una **Eleccion** si es correcta. La **Eleccion** afecta a la **Persona**, reflejando el impacto de la decisión tomada.