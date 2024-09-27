# Reto 001

### Crear diagrama de clases de La Sombra

## **Plant UML**

### Diagrama de clases

    @startuml
        package "Sombra" {

            FocoDeLuz -- Luz : "Genera"

            Luz -- Objeto : "Incide"

            Objeto -- Sombra : "Produce"

            Sombra-- Superficie: "Se proyecta"

        }
    @enduml


### Sombra

|Ejercicio|Codigo|Diagrama|
|-|-|:-:|
|1. Diagrama de clases|    
    @startuml
        package "Sombra" {

            FocoDeLuz -- Luz : "Genera"

            Luz -- Objeto : "Incide"

            Objeto -- Sombra : "Produce"

            Sombra-- Superficie: "Se proyecta"

        }
    @enduml
    |![](\entregas\garciaDiego\Imagenes\Sombra.svg)
|2. Diagrama de objetos, dos focos y una persona|[Código](/entregas/garciaDiego/Reto002/Sombra2.puml)|![](\entregas\garciaDiego\Imagenes\Sombra2.svg)
|3. Diagrama de objetos, dos focos y una persona|[Código](/entregas/garciaDiego/Reto002/Sombra3.puml)|![](\entregas\garciaDiego\Imagenes\Sombra3.svg)
|4. Diagrama de objetos, dos focos y una persona|[Código](/entregas/garciaDiego/Reto002/Sombra4.puml)|![](\entregas\garciaDiego\Imagenes\Sombra4.svg)


