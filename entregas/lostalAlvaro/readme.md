# Reto 10-10: Diagrama de Elección

## Introducción

En este ejercicio he desarrollado dos diagramas UML que representan el proceso de votación y elección de un delegado de clase. Los diagramas muestran tanto una visión general de los elementos involucrados como una instancia específica del proceso en un contexto concreto.

## Diagrama de Clases: Votación

### Diagramas

| Nombre                            | Imagen                                                                 |
|-----------------------------------|------------------------------------------------------------------------|
| Diagrama de Clases de Votación    | ![Diagrama de Clases Votación](/entregas/lostalAlvaro/img/votacionClases.svg)    |

### Explicación

- **Diagrama de Clases de Votación**: Este diagrama representa las clases **Votante**, **Postulante**, **Voto**, **Elección**, **Urna** y **Supervisor**. 
  - Los **Votantes** emiten un **Voto** que está dirigido a un **Postulante** (o candidato).
  - El **Voto** se almacena en una **Urna**, que es utilizada en una **Elección**.
  - La **Elección** incluye a varios **Postulantes**.
  - El **Supervisor** supervisa la **Urna**, pero también puede emitir su propio **Voto**, ya que también actúa como votante.

## Diagrama de Objetos: Elección de Delegado

### Diagramas

| Nombre                             | Imagen                                                                 |
|------------------------------------|------------------------------------------------------------------------|
| Diagrama de Objetos de Elección    | ![Diagrama de Objetos Elección](/entregas/lostalAlvaro/img/votacionObjetos.svg)  |

### Explicación

- **Diagrama de Objetos de Elección de Delegado**: Este diagrama muestra una instancia específica del proceso de votación para la elección de un delegado de clase.
  - Los votantes incluyen a **Alvaro Lostal**, quien emite su **VotoAlvaro**.
  - Los postulantes incluyen a **Mario del Río**, **Diego García**, **Maura Martínez**, **Javier Salmerón** y **Elías Alcorcón**, quienes participan en la elección como candidatos.
  - El **VotoAlvaro** se almacena en la **UrnaAula**, que está bajo la supervisión de **Alejandro Viñas**.
  - La elección en cuestión es la **EleccionDelegadoClase**.