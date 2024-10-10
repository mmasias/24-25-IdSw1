# Vocabulario del Diagrama de Clases

## Clases

### 1. Alumno
- Representa a los estudiantes de la institución.
- **Relaciones:**
  - **Candidato:** El `Candidato` es un tipo de `Alumno` (herencia).
  - **Secretario:** Un `Alumno` puede estar asociado con un `Secretario` (agregación).
  - **Voto:** Un `Alumno` está relacionado con un `Voto` (dependencia).

### 2. Candidato
- Un `Candidato` es un alumno que participa en las elecciones.
- **Relaciones:**
  - **Alumno:** El `Candidato` hereda de `Alumno`.
  - **ActaDeEleccion:** El `Candidato` está relacionado con el `ActaDeEleccion` (dependencia).

### 3. Profesor
- Representa al personal docente con un papel en el proceso electoral.
- **Relaciones:**
  - **Presidente:** Un `Profesor` puede estar relacionado con el rol de `Presidente` (agregación invertida).

### 4. Presidente
- El `Presidente` preside el proceso electoral.
- **Relaciones:**
  - **Profesor:** El `Presidente` es un tipo de `Profesor`.
  - **MesaElectoral:** El `Presidente` está directamente relacionado con la `MesaElectoral`.

### 5. Secretario
- Un `Alumno` que asume el rol de organizar el proceso electoral.
- **Relaciones:**
  - **Alumno:** El `Secretario` está asociado con un `Alumno` (agregación).
  - **MesaElectoral:** El `Secretario` está relacionado con la `MesaElectoral`.
  - **ActaDeEleccion:** El `Secretario` tiene un rol en la creación del `ActaDeEleccion` (dependencia).

### 6. MesaElectoral
- Coordina y gestiona el proceso de votación.
- **Relaciones:**
  - **Voto:** La `MesaElectoral` recibe los votos.
  - **Presidente:** El `Presidente` forma parte de la `MesaElectoral`.
  - **Secretario:** El `Secretario` también forma parte de la `MesaElectoral`.
  - **ActaDeEleccion:** La `MesaElectoral` está relacionada con la creación del `ActaDeEleccion`.

### 7. Voto
- Representa la acción de votar en el proceso electoral.
- **Relaciones:**
  - **Alumno:** Los alumnos generan los votos.
  - **MesaElectoral:** Los votos son procesados por la `MesaElectoral`.
  - **ActaDeEleccion:** Los votos son registrados en el `ActaDeEleccion`.

### 8. ActaDeEleccion
- Documento que formaliza los resultados del proceso electoral.
- **Relaciones:**
  - **Voto:** Los votos se contabilizan en el `ActaDeEleccion`.
  - **MesaElectoral:** La `MesaElectoral` está relacionada con el `ActaDeEleccion`.
  - **Secretario:** El `Secretario` está vinculado con la creación del acta.
  - **Candidato:** Los `Candidatos` participan en el proceso que lleva a la creación del acta.

## Tipos de Relaciones

- **Herencia (`<|--`)**: Representa una relación de especialización. Un ejemplo es que `Candidato` hereda de `Alumno`.
- **Agregación (`o..`)**: Indica que una clase está compuesta por otras, pero estas pueden existir independientemente. Por ejemplo, `Alumno` y `Secretario`.
- **Asociación (`--`)**: Relación directa entre dos clases. Por ejemplo, entre `Voto` y `MesaElectoral`.
- **Dependencia (`..`)**: Una clase depende de otra para algunas operaciones, pero no implica una relación permanente. Por ejemplo, entre `Candidato` y `ActaDeEleccion`.
