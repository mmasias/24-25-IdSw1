# Glosario y Relaciones Importantes

Hemos realizado una votación en nuestra clase para elegir a un delegado y a un subdelegado, éstas son sus partes:
## Sistema de Votación

### Clases

#### Persona
- **Descripción**: Representa a cada miembro de la clase. Puede ser tanto un votante como un candidato en la elección.
- **Atributos**:
  - `nombre`: El nombre del estudiante.
  - `esDelegado`: Indica si la persona ha sido elegida como delegado.
  - `esSubdelegado`: Indica si la persona ha sido elegida como subdelegado.
- **Relaciones**:
  - Relacionada con `Voto` como votante.
  - Relacionada con `Voto` como candidato.

#### Voto
- **Descripción**: Cada voto emitido en la elección. Se registra quién vota (votante) y por quién se vota (candidato).
- **Atributos**:
  - `votante`: La persona que ha emitido el voto.
  - `candidato`: La persona a la que va dirigido el voto.
- **Relaciones**:
  - Relacionado con `Persona` como votante y candidato.

#### Urna
- **Descripción**: Contenedor donde se almacenan todos los votos emitidos durante la elección.
- **Atributos**:
  - `votos`: Lista de objetos de tipo `Voto` que representan todos los votos almacenados.
- **Relaciones**:
  - Contiene una lista de `Voto`.

#### Elección
- **Descripción**: El proceso en el cual se eligen al delegado y subdelegado de la clase.
- **Atributos**:
  - `urna`: La urna que contiene todos los votos emitidos.
  - `totalVotantes`: Número total de personas que participaron en la votación.
  - `delegado`: Persona elegida como delegado.
  - `subdelegado`: Persona elegida como subdelegado.
- **Métodos**:
  - `contarVotos()`: Cuenta los votos almacenados en la urna.
  - `determinarGanadores()`: Determina quién es elegido delegado y subdelegado basándose en los votos.
- **Relaciones**:
  - Contiene la `Urna` con los votos.
  - Relacionado con `Persona` como delegado y subdelegado.
  - Supervisado por `MesaElectoral`.

#### MesaElectoral
- **Descripción**: Grupo de personas encargadas de supervisar el proceso de elección para asegurar que todo se realice de manera justa.
- **Atributos**:
  - `miembros`: Lista de personas que componen la mesa electoral.
- **Métodos**:
  - `supervisarElección()`: Supervisa el desarrollo de la elección.
- **Relaciones**:
  - Compuesta por miembros que son `Persona`.
  - Supervisa el proceso de `Elección`.

---

### Relaciones Globales

- **Persona**:
  - Se relaciona con `Voto` como votante y candidato.
- **Urna**:
  - Almacena una lista de `Voto` emitidos por `Persona`.
- **Elección**:
  - Depende de la `Urna` para contener los votos.
  - Define al `delegado` y `subdelegado` que son instancias de `Persona`.
  - Es supervisada por la `MesaElectoral`.
- **MesaElectoral**:
  - Sus miembros son `Persona`.
  - Supervisa el proceso de la `Elección`.

---

