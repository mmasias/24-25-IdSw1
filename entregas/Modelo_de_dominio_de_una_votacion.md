## MODELO DE UNA VOTACION
A continuacion se muestra el modelo de domino de una votacion en la cual se muestra como, 
en un proceso electivo, se relacionan los distintos elementos:
### Votante
El votante, debido a sus características tiene lo siguiente:
- Un ID, su dni o identificador, este dato puede ser omitible en algunos contextos
- Nombre y apellido
- Estado en la votacion; siendo este si ya voto o no
  
  Se relaciona con los distintos elementos votando al candidato y emitiendo un voto, asi
  como permitiendo la realizacion de la votacion, ya que sin el no hay votacion
### Candidato
Es quien se presenta a la votacion para ser elegido, tiene las siguientes características:
- ID, nombre y apellido; al igual que el votante
- El número de votos, conocido por él al finalizar la votacion
- El resultado de la votacion, siendo este si sale victorioso o no
  
  Sus relaciones con los otros elementos son el "recibir los votos", el postularse a las
  elecciones y ser incluido en los documentos de la misma
### Eleccion
Es el proceso a realizar; este incluye:
- Un ID identificativo del proceso; importante a la hora de documentarlo y encontrar los resultados de cara al futuro
- Una fecha de inicio y de fin
- El estado, siendo este iniciado o terminado
- Un recuento de votos  

  Se relaciona con el resto de elementos ya que contiene los votos emitidos por los votantes,
  a los candidatos, asi como que precisa de un presidente que la dirija y un secretatio que cuente los votos
  
### Voto
Esta contenido en la eleccion:
- Tiene un ID de voto
- Fecha y hora de emision del mismo  

  Se relaciona con los otros elementos siendo contenida en las elecciones, recibida por el candidato y emitida por el votante
  
### Secretario
Es un elemento clave de la eleccion:
- Tiene un ID
- Nombre y apellido  

  Se relaciona con los votos contadolos y permitiendo la realizaciond e la eleccion ya que sin el no se puede realizar el proceso
  
### Presidente
 Es quien redacta el acta tras el proceso electivo, tiee lo siguiente:
 -ID
 - Nombre y apellido  

Es quien anuncia el ganador y consulta los votos emitidos por los votantes y leidos por el secretario, a su vez es quien dirige el proceso  

[img1] : C:\UNIVERSIDADv2\24-25\3º\IdSw1\Ejercicios\MODELAJE\src\ejercicio3\VOTACION-Modelo_del_Dominio__Elección_de_Delegado.png
