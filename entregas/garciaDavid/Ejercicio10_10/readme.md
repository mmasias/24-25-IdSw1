# Glosario - Modelo de Dominio para un Acto de Votación

## 1. Clase
- **Definición**: Conjunto de estudiantes que participan en el proceso de votación.
- **Rol**: Agrupa a los estudiantes y organiza la votación para elegir a un delegado.
- **Estados**:
  - Sin votación
  - Votación en curso
  - Votación finalizada

## 2. Estudiante
- **Definición**: Individuo que forma parte de una clase y puede participar en la votación como votante o candidato.
- **Rol**: El estudiante emite su voto para elegir a un candidato.
- **Estados**:
  - No ha votado
  - Ha votado

## 3. Candidato
- **Definición**: Estudiante postulado para ser delegado de la clase.
- **Rol**: Compite en la votación para ser elegido delegado.
- **Estados**:
  - Cero votos
  - Votos asignados
  - Delegado(Si/No)

## 4. Votación
- **Definición**: Proceso en el que los estudiantes emiten sus votos para elegir a un delegado.
- **Rol**: Coordina el acto de votar y registra los votos emitidos.
- **Estados**:
  - Abierta (los estudiantes pueden votar)
  - Cerrada (se termina el proceso de emisión de votos)
  - Estado
  - Proceso
## 5. Voto
- **Definición**: Acto mediante el cual un estudiante expresa su elección por un candidato.
- **Rol**: Cada estudiante emite un voto que se suma al candidato seleccionado.
- **Estados**:
  - No emitido
  - Emitido

## 6. Resultado
- **Definición**: Resultado final de la votación que muestra el candidato ganador.
- **Rol**: Calcula el candidato con mayor número de votos y lo declara como ganador.
- **Estados**:
  - En espera (no calculado)
  - Calculado (ganador determinado)

