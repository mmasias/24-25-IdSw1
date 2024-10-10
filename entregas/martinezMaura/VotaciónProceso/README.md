# Descripción del Modelo del Dominio

Este modelo del dominio representa el proceso de votación para elegir un delegado en un salón de clases universitario. Incluye las siguientes entidades clave:

## Personas
Están modeladas como estudiantes, profesores y secretarios, cada una con roles específicos en el proceso de votación.

- **Estudiantes**: Participan en la votación eligiendo a uno de los candidatos como delegado.
- **Profesor**: Inicia y cierra el proceso de votación.
- **Secretario**: Cuenta los votos depositados en la urna.

## Urna y Votos
La urna es el objeto que recibe los votos, y cada voto está asociado a un estudiante y un delegado votado. Los delegados son estudiantes que han sido votados.

## Flujo del Proceso
1. El profesor abre la votación.
2. Los estudiantes emiten sus votos.
3. El secretario cuenta los votos para determinar quién ha sido elegido delegado.
4. Finalmente, se anuncia al delegado con más votos.

## Diagrama de Clases
Define las relaciones entre las diferentes entidades del sistema.

## Diagrama de Estados
Muestra los estados por los que pasa el proceso de votación, desde la apertura hasta el conteo de votos y el anuncio del resultado.

## Diagrama de Objetos
Representa instancias del modelo en un caso específico de votación, donde varios estudiantes han emitido sus votos y un delegado ha sido elegido.

---

