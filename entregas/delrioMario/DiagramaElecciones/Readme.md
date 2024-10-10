# Proceso de Votación

Este proyecto contiene representaciones del proceso de votación utilizando diagramas UML, específicamente de objetos y de estados, que ayudan a visualizar los componentes involucrados y su flujo. A continuación se describe cada diagrama y su propósito.

## Diagrama de clases

Este diagrama describe de manera abstracta en que consiste una votacion a delegado

### Código PUML:
```puml
@startuml

class voto
class votantes
class candidatos
class recuento

candidatos -> votantes : se presentan a
votantes -> voto : derecho a votos
voto ->  recuento : se recojen en
recuento .... candidatos : elegido

@enduml

## Diagrama de Objetos

Este diagrama describe las relaciones entre los diferentes objetos que forman parte del proceso de votación, como votantes, candidatos, los votos y el recuento de votos.

### Código PUML:
```puml
@startuml
object Votantes {
}
object Candidatos {
}
object Voto {
}
object Recuento {
}

Candidatos --> Votantes : "se presentan a"
Votantes --> Voto : "derecho a votos"
Voto --> Recuento : "se recogen en"
Recuento ..> Candidatos : "elegido"
@enduml

