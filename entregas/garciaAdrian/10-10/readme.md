# Sistema de Votación para Delegados

Este repositorio presenta un modelo del proceso de votación para elegir un delegado. Se incluyen diagramas que representan los estados, clases y objetos involucrados en el proceso de votación.

## Contenido

1. Diagrama de Estados
2. Diagrama de Clases
3. Diagrama de Objetos
4. Descripción General

---

## Diagrama de Estados

El diagrama de estados describe los diferentes estados del proceso de votación:

- **EsperandoVotantes**: Estado inicial donde se espera la llegada de votantes.
- **Votando**: Estado en el que los votantes emiten sus votos.
- **Recuento**: Estado en el que se cuentan los votos después de finalizar la votación.
- **Resultado**: Estado final que muestra los resultados de la votación.

---

## Diagrama de Clases

El diagrama de clases define las entidades clave en el sistema:

- **Votante**: Representa a los votantes, con atributos como nombre y el método para emitir votos.
- **Candidato**: Representa a los candidatos, con atributos como nombre y el total de votos recibidos.
- **Votacion**: Clase que gestiona el proceso de votación, incluyendo métodos para iniciar, finalizar y contar votos.
- **Resultado**: Clase que contiene la información sobre el total de votos y los candidatos, mostrando los resultados finales.

---

## Diagrama de Objetos

El diagrama de objetos proporciona una representación más detallada y específica del sistema:

- **Votación**: Estado de la votación y total de votos contabilizados.
- **Votantes**: Ejemplos de votantes con su elección específica.
- **Candidatos**: Ejemplos de candidatos y el número de votos que han recibido.
- **Resultado Final**: Resumen de los resultados con el total de votos y los candidatos involucrados.

Las relaciones muestran cómo cada votante participa en la votación, votando por un candidato específico, y cómo estos votos contribuyen al resultado final.

---

## Descripción General

Este modelo es una representación simplificada de un proceso de votación, que puede ser utilizado como base para desarrollar un sistema más complejo. Proporciona una comprensión clara de las interacciones entre votantes, candidatos y el sistema de votación en general.


