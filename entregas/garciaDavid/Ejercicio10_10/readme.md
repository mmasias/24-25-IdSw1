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

## 4. Votación
- **Definición**: Proceso en el que los estudiantes emiten sus votos para elegir a un delegado.
- **Rol**: Coordina el acto de votar y registra los votos emitidos.
- **Estados**:
  - Abierta (los estudiantes pueden votar)
  - Cerrada (se termina el proceso de emisión de votos)

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

## 7. Estado de la Votación
- **Definición**: Indica si la votación está en curso o finalizada.
- **Rol**: Controla el flujo del proceso de votación.
- **Estados**:
  - Abierta
  - Cerrada

## 8. Delegado
- **Definición**: Estudiante elegido para representar a la clase.
- **Rol**: El delegado representa a la clase tras haber sido elegido mediante el proceso de votación.
- **Estados**:
  - No delegado
  - Elegido como delegado

## 9. Proceso de Votación
- **Definición**: El flujo completo desde la apertura de la votación hasta la declaración del resultado.
- **Rol**: Coordina la participación de los estudiantes en la elección del delegado.
- **Estados**:
  - Inicializado
  - En curso
  - Finalizado

## 10. Conteo de Votos
- **Definición**: Proceso que suma los votos recibidos por cada candidato.
- **Rol**: Determina el número de votos obtenidos por cada candidato y quién es el ganador.
- **Estados**:
  - No iniciado
  - En progreso
  - Finalizado

