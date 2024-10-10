# Glosario y Relaciones Importantes

Hemos realizado una votacion en clase para elegir delegado y subdelegado y en esto podríamos dividirlo: 

SistemaVotación:
  Clases:
    - Persona:
        Descripción: Representa a cada miembro de la clase. Puede ser tanto un votante como un candidato en la elección.
        Atributos:
          - nombre: El nombre del estudiante.
          - esDelegado: Indica si la persona ha sido elegida como delegado.
          - esSubdelegado: Indica si la persona ha sido elegida como subdelegado.
        Relaciones:
          - Voto: Relacionado como votante.
          - Voto: Relacionado como candidato.

    - Voto:
        Descripción: Cada voto emitido en la elección. Se registra quién vota (votante) y por quién se vota (candidato).
        Atributos:
          - votante: La persona que ha emitido el voto.
          - candidato: La persona a la que va dirigido el voto.
        Relaciones:
          - Persona: Está asociado a una Persona como votante y a otra Persona como candidato.

    - Urna:
        Descripción: Contenedor donde se almacenan todos los votos emitidos durante la elección.
        Atributos:
          - votos: Lista de objetos de tipo Voto que representan todos los votos almacenados.
        Relaciones:
          - Voto: Contiene una lista de votos.

    - Elección:
        Descripción: El proceso en el cual se eligen al delegado y subdelegado de la clase.
        Atributos:
          - urna: La urna que contiene todos los votos emitidos.
          - totalVotantes: Número total de personas que participaron en la votación.
          - delegado: Persona elegida como delegado.
          - subdelegado: Persona elegida como subdelegado.
        Métodos:
          - contarVotos(): Cuenta los votos almacenados en la urna.
          - determinarGanadores(): Determina quién es elegido delegado y subdelegado basándose en los votos.
        Relaciones:
          - Urna: Contiene la Urna donde se almacenan los votos.
          - Persona: Relacionado con Persona como delegado.
          - Persona: Relacionado con Persona como subdelegado.
          - MesaElectoral: La elección está supervisada por la MesaElectoral.

    - MesaElectoral:
        Descripción: Grupo de personas encargadas de supervisar el proceso de elección para asegurar que todo se realice de manera justa.
        Atributos:
          - miembros: Lista de personas que componen la mesa electoral.
        Métodos:
          - supervisarElección(): Supervisa el desarrollo de la elección.
        Relaciones:
          - Persona: Está compuesta por miembros que son Personas.
          - Elección: Supervisan el proceso de Elección.

  RelacionesGlobales:
    - Persona:
        - Voto: Cada Persona puede ser tanto un votante como un candidato.
    - Urna:
        - Voto: Almacena una lista de votos emitidos por Personas.
    - Elección:
        - Urna: La Elección depende de la Urna para contener los votos.
        - Persona: Define al delegado y subdelegado elegidos.
        - MesaElectoral: Supervisa la Elección.
    - MesaElectoral:
        - Persona: Los miembros son Personas.
