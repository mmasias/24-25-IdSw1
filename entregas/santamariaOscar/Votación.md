# Acción de ejercer el derecho a voto

## Contexto
El acto de votar es una acción fundamental en el proceso democrático mediante la cual las personas expresan su voluntad y eligen a sus representantes o toman decisiones sobre asuntos de interés público. El derecho al voto se considera un derecho cívico básico y una herramienta esencial para la participación en la vida política de una comunidad, ya sea en elecciones generales, referendos, o elecciones locales.

## Diagramas
|**Diagrama de Clases**| **Diagrama de Objetos**|
|----------------------|------------------------|
|![Diagrama de Clases](https://github.com/user-attachments/assets/532dbc09-5628-44cc-92f0-07cb1b9d7740)|![Diagrama de Objetos](https://github.com/user-attachments/assets/87e9e892-8443-43b3-b772-1a3bf7b588f5)|


### Explicación del Diagrama de Clases
El **Diagrama de Clases** representa las entidades principales y sus relaciones en el proceso de votación. Las clases incluidas en el diagrama son:

- **Elección**: Representa un evento electoral en el que los votantes pueden participar. Contiene información básica como el `Nombre`, `Fecha`. 
  
- **Votante**: Define a las personas habilitadas para emitir un voto. Los atributos `Nombre`, `DNI` y `HaVotado` identifican al votante y permiten saber si ya ha emitido su voto.

- **Voto**: Representa el acto de votar y se asocia tanto con un votante como con un candidato. 

- **Candidato**: Define a las personas que compiten en una elección. Incluye atributos como `Nombre`, `Partido`, y `NumeroVotos` para representar la información de los candidatos y el número de votos recibidos.

- **MesaElectoral**: Representa el lugar físico o virtual donde se realizan las votaciones. Contiene atributos como `Localizacion`, y `NumeroVotantes`.

Las relaciones entre estas clases permiten modelar un sistema de votación, desde la inscripción de candidatos y votantes, hasta la emisión y conteo de votos.


### Explicación del Diagrama de Objetos
El **Diagrama de Objetos** representa instancias específicas de las clases en un momento determinado. Muestra cómo interactúan entre sí para realizar una votación concreta. Por ejemplo, se pueden ver:

- Instancias de `Votante` con valores únicos para cada votante (`Nombre` y `DNI`).
- Instancias de `Candidato` con valores específicos para el `Nombre` y `Partido`.
- Una instancia de `Voto` que se asocia a un `Candidato` y a un `Votante` en un momento específico (`FechaHora`).

Este diagrama ilustra cómo las instancias de las clases colaboran para llevar a cabo una votación real.

## Caso Específico: Elección de Delegado de Clase
En el contexto de una **elección de delegado de clase**, el proceso se desarrolla de la siguiente manera:

1. **Elección**: Se crea una nueva elección con el nombre "Elección de Delegado de Clase" y se establece la fecha de la votación.

2. **Candidatos**: Los estudiantes interesados en ser delegados se inscriben como candidatos. Cada candidato tiene un nombre y puede representar una propuesta específica (e.g., mejora de recursos educativos, organización de actividades).

3. **Votantes**: Todos los estudiantes de la clase tienen derecho a votar. Se registran como `Votantes` con su `Nombre` y un identificador único.

4. **Mesa Electoral**: Se organiza una mesa electoral en el aula, donde los estudiantes se presentan para emitir su voto. La `MesaElectoral` valida que cada estudiante sea parte de la clase y no haya votado previamente.

5. **Voto**: Cada estudiante emite un voto seleccionando al candidato de su preferencia. El `Voto` se asocia al votante y al candidato correspondiente. 

6. **Resultados**: Al finalizar la elección, se cierra la votación, se cuentan los votos y se declara el candidato con el mayor número de votos como el delegado de la clase.

Este caso específico de elección de delegado de clase se modela de forma similar al diagrama de clases y objetos descrito, pero adaptado al entorno educativo, donde los votantes son estudiantes y los candidatos son compañeros de clase.
