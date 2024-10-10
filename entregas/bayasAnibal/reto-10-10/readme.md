# Glosario del Diagrama de Clases

## 1. Votante
**Descripción**: Representa a una persona que participa en una votación emitiendo un voto.

**Atributos**:
- `id`: Entero que identifica de manera única al votante.
- `nombre`: Cadena de caracteres que representa el nombre del votante.
- `haVotado`: Booleano que indica si el votante ha emitido su voto (`true` si ya votó, `false` si aún no lo ha hecho).

**Relaciones**:
- El `Votante` **emite** un `Voto`.

---

## 2. Voto
**Descripción**: Representa el acto de votación en el que un votante selecciona un candidato.

**Atributos**:
- `fecha`: Fecha en la que se emite el voto.
- `candidato`: El candidato por el cual el voto ha sido emitido.

**Métodos**:
- `registrarVoto()`: Método que registra oficialmente el voto en el sistema.

**Relaciones**:
- El `Voto` es **para** un `Candidato`, lo que significa que el voto va dirigido a uno de los candidatos de la votación.

---

## 3. Votación
**Descripción**: Representa el proceso completo de votación, que tiene un inicio y un fin, en el cual los votantes eligen a uno o más candidatos.

**Atributos**:
- `fechaInicio`: Fecha en la que inicia la votación.
- `fechaFin`: Fecha en la que finaliza la votación.

**Métodos**:
- `realizarVotacion()`: Inicia y gestiona el proceso de votación.
- `contarVotos()`: Realiza el conteo de los votos emitidos para determinar el ganador o los resultados de la votación.

**Relaciones**:
- La `Votación` **contiene** a varios `Candidatos`.
- Los `Candidatos` **participan en** una `Votación`.

---

## 4. Candidato
**Descripción**: Representa a una persona que se postula para ser elegida en una votación.

**Atributos**:
- `id`: Entero que identifica de manera única al candidato.
- `nombre`: Nombre del candidato.
- `votosObtenidos`: Entero que representa la cantidad de votos que el candidato ha recibido.

**Métodos**:
- `proponerPlan()`: Permite al candidato presentar un plan o propuesta a los votantes como parte de su campaña.

**Relaciones**:
- Los `Candidatos` **participan en** una `Votación`.
- Los `Candidatos` también reciben votos, y el `Voto` está dirigido **para** un `Candidato`.

---

## Resumen de Relaciones entre Clases:
- **Votante emite un Voto**: Un votante puede emitir un voto. La relación indica que el votante es responsable de generar un voto en el sistema.
- **Voto es para un Candidato**: El voto está destinado a un candidato específico, lo que significa que se utiliza para expresar apoyo por ese candidato.
- **Votación contiene Candidatos**: Una votación incluye múltiples candidatos que participan en ella. Cada votación tiene una lista de candidatos disponibles.
- **Candidato participa en Votación**: Un candidato participa en una votación, lo que significa que es una opción que los votantes pueden elegir durante el proceso de votación.

---

## Ejemplo de Flujo:
1. Un `Votante` (por ejemplo, Juan) decide emitir un `Voto`.
2. El `Voto` se registra para un `Candidato` específico (por ejemplo, Ana).
3. Este proceso ocurre dentro del marco de una `Votación` (que tiene un período de tiempo y puede incluir varios candidatos como Ana y Luis).
4. Los `Candidatos` participan en la votación esperando ser elegidos por los votantes.
