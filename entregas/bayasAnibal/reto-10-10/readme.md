# Glosario del Diagrama de Clases

## Votante
- **Descripción:** Persona que emite un voto.
- **Atributos:**  
  - `id`: Identificador único.  
  - `nombre`: Nombre del votante.  
  - `haVotado`: Indica si ya votó (`true` o `false`).  
- **Relaciones:** Emite un Voto.

## Voto
- **Descripción:** Representa el voto de un votante hacia un candidato.
- **Atributos:**  
  - `fecha`: Fecha del voto.  
  - `candidato`: Candidato seleccionado.  
- **Métodos:**  
  - `registrarVoto()`: Registra el voto en el sistema.  
- **Relaciones:** Va dirigido a un Candidato.

## Votación
- **Descripción:** Proceso donde los votantes eligen candidatos en un período determinado.
- **Atributos:**  
  - `fechaInicio`: Fecha de inicio.  
  - `fechaFin`: Fecha de fin.  
- **Métodos:**  
  - `realizarVotacion()`: Inicia el proceso.  
  - `contarVotos()`: Cuenta los votos para determinar resultados.  
- **Relaciones:** Contiene varios Candidatos.

## Candidato
- **Descripción:** Persona postulada para ser elegida.
- **Atributos:**  
  - `id`: Identificador único.  
  - `nombre`: Nombre del candidato.  
  - `votosObtenidos`: Número de votos recibidos.  
- **Métodos:**  
  - `proponerPlan()`: Presenta su propuesta.  
- **Relaciones:** Participa en una Votación y recibe votos.

## Resumen de Relaciones
- **Votante emite un Voto**: Un votante registra su voto.
- **Voto es para un Candidato**: El voto está destinado a un candidato.
- **Votación contiene Candidatos**: Una votación incluye varios candidatos.
- **Candidato participa en Votación**: Los candidatos son opciones para los votantes.


## Ejemplo de Flujo:
1. Un `Votante` (por ejemplo, Juan) decide emitir un `Voto`.
2. El `Voto` se registra para un `Candidato` específico (por ejemplo, Ana).
3. Este proceso ocurre dentro del marco de una `Votación` (que tiene un período de tiempo y puede incluir varios candidatos como Ana y Luis).
4. Los `Candidatos` participan en la votación esperando ser elegidos por los votantes.
