# Reto 001

### Mejorar el diagrama de clases realizado en clase

## **Plant UML**

    @startuml
        package "LIGA" {
    
            Normas -- Arbitro : "Aplica"
            
            Arbitro -- Partido: "Supervisa"
            
            Partido -- Estadio : "Donde se compite"
            
            Equipo .. Estadio : "Tiene"
            
            Equipo -- Alineación : "Elige"
            
            Partido -- Alineación: "Compite"
            
            Jornada -- Partido : "Contiene"
            
            Temporada -- Jornada : "Tiene"
            
            Ranking -- Jornada : "Tiene"
            
            Ranking -- Equipo : "Se clasifica"
            
            Ranking -- Premio : "Tiene"
            
            Afición .. Estadio : "lo ven en"
            
            Afición -- Equipo : "Apoyan"
            
            Jugador -- Equipo : "Contiene"
            
            Jugador -- Alineación : "Contiene"
            
            Federación -- Requisitos : "Pone"
            
            Requisitos -- Equipo : "Cumple"
            
            Federación -- Temporada : "Organiza"
            
            Federación -- Arbitro : "Asigna"
            
            Afición -- Partido : "Asiste a"
    
    
    }
    @enduml


||
|-:|

![](/entregas/garciaDiego/Imagenes/PUML_LaLiga_IGPWS.png)


## **Clases y Relaciones**

1. **Normas __--__ Arbitro: "Aplica"**
   - El árbitro es responsable de aplicar las normas establecidas para garantizar el correcto desarrollo de los partidos.

2. **Arbitro __--__ Partido: "Supervisa"**
   - El árbitro supervisa el partido, asegurándose de que se respeten las reglas y gestionando el juego.

3. **Partido __--__ Estadio: "Donde se compite"**
   - Cada partido se lleva a cabo en un estadio específico, que es el lugar de la competencia.

4. **Equipo __..__ Estadio: "Tiene"**
   - Un equipo tiene un estadio donde juega sus partidos como local, aunque esta relación es una asociación débil.

5. **Equipo __--__ Alineación: "Elige"**
   - El equipo elige su alineación, que es la selección de jugadores que participarán en un partido específico.

6. **Partido __--__ Alineación: "Compite"**
   - Durante un partido, las alineaciones de ambos equipos compiten entre sí.

7. **Jornada __--__ Partido: "Contiene"**
   - Una jornada de la liga contiene varios partidos que se juegan en un periodo determinado.

8. **Temporada __--__ Jornada: "Tiene"**
   - Una temporada de liga está compuesta por múltiples jornadas a lo largo del tiempo.

9. **Ranking __--__ Jornada: "Tiene"**
   - Cada jornada se refleja en un ranking que clasifica a los equipos según su rendimiento.

10. **Ranking __--__ Equipo: "Se clasifica"**
    - Los equipos se clasifican en el ranking basado en sus resultados en los partidos.

11. **Ranking __--__ Premio: "Tiene"**
    - El ranking puede determinar premios que se otorgan a los equipos en función de su posición al final de la temporada.

12. **Afición __..__ Estadio: "lo ven en"**
    - Los aficionados ven los partidos en el estadio, indicando una relación de asistencia.

13. **Afición __--__ Equipo: "Apoyan"**
    - La afición apoya a un equipo, siendo una parte importante del ambiente y la motivación durante los partidos.

14. **Jugador __--__ Equipo: "Contiene"**
    - Un equipo contiene a varios jugadores que son parte de su plantilla.

15. **Jugador __--__ Alineación: "Contiene"**
    - Una alineación contiene a los jugadores que han sido seleccionados para participar en un partido específico.

16. **Federación __--__ Requisitos: "Pone"**
    - La federación establece requisitos que los equipos deben cumplir para participar en la liga.

17. **Requisitos __--__ Equipo: "Cumple"**
    - Los equipos deben cumplir con los requisitos establecidos por la federación para poder competir.

18. **Federación __--__ Temporada: "Organiza"**
    - La federación organiza las temporadas de la liga, definiendo el formato y las reglas del torneo.

19. **Federación __--__ Arbitro: "Asigna"**
    - La federación se encarga de asignar árbitros a los partidos, asegurando que se cumpla la normativa.

20. **Afición __--__ Partido: "Asiste a"**
    - Los aficionados asisten a los partidos, apoyando a sus equipos en el lugar de la competencia.


