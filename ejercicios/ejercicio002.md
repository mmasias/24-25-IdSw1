# Ejercicio 002

Modelar utilizando los artefactos que considere pertinentes:

- La sombra

## iteracion 1
```csharp
@startuml

class FuenteDeLuz
class Objeto
class Sombra
class Superficie

FuenteDeLuz -- Objeto
Objeto -- Sombra
Sombra -- Superficie


@enduml
```

![sombraIteracion1.png](imagenes\sombraIteracion1.png)

```csharp
@startuml
title Sombra

object person1

object foco1
object foco2

object Sombra1
object Sombra2

object superficie

foco1 -- person1
foco2 -- person1

person1 -- Sombra1
person1 -- Sombra2

Sombra2 -- superficie
Sombra1 -- superficie


@enduml

```


## iteracion 2
```csharp
@startuml

class FuenteDeLuz
class Objeto
class Sombra
class Superficie

FuenteDeLuz -- Objeto
Objeto -- Sombra
Sombra -- Superficie


@enduml
```

![sombraIteracion2.png](imagenes\sombraIteracion2.png)


## iteracion 3
```csharp
@startuml

class FuenteDeLuz
class Objeto
class Sombra
class Superficie


FuenteDeLuz -- Objeto
Objeto -- Sombra
Objeto .. Sombra
Sombra -- Superficie
FuenteDeLuz .. Superficie

@enduml
```

![sombraIteracion3.png](imagenes\sombraIteracion3.png)

### Diagramas de objetos

- una persona, dos focos 

![Diagrama de Objetos - una persona, dos focos](imagenes/diagramaObjetosIteracion1Sombra.png)
- dos personas, dos focos

![Diagrama de Objetos - dos personas, dos focos](imagenes/diagramaObjetosIteracion1_2Sombra.png)
