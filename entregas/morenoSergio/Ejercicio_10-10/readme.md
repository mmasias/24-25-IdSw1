# Sistema de Votación - Modelo de Dominio

### Diagrama de Clases

El diagrama de clases muestra las principales entidades del sistema y sus relaciones. Las entidades incluyen:

- **Votante**: Persona que emite un voto.
- **Candidato**: Persona que puede ser votada en la elección.
- **Elección**: Proceso de votación que agrupa votantes y candidatos.
- **Distrito**: Área geográfica que contiene varias mesas de votación.
- **Mesa**: Lugar donde votan los votantes y se deposita el voto en una urna.
- **Urna**: Contenedor de votos.
- **Voto**: Representación del acto de votar.
- **Resultado**: Contabiliza los votos de los candidatos.

### Diagrama de Estados

El diagrama de estados muestra cómo cambia el estado de una elección:

- **Configurando**: Inicialmente, la elección está en configuración, donde se agregan candidatos y votantes.
- **En Progreso**: Una vez iniciada la votación, la elección entra en este estado.
- **Cerrada**: Cuando se cierra la votación, el estado cambia a "Cerrada".
- **Mostrando Resultados**: Después de cerrar, los resultados se calculan y muestran.

### Diagrama de Objetos

El diagrama de objetos muestra una instancia específica de las clases. En este caso, representa una votación en curso con un votante, un candidato, una urna y un voto.
