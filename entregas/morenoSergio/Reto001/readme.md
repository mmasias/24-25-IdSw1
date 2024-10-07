En cuanto al arcoiris:
- Se han añadido atributos como intensidad, longitudDeOnda para la clase Luz, y atributos como temperatura, claridad para la clase Agua.
- Se han agregado más relaciones entre clases. Por ejemplo, ahora Refraccion y Dispersion están conectadas ya que ambas son responsables de la separación de colores.
- Reflexion y Dispersion ahora interactúan modificando el ángulo de dispersión, lo que tiene un impacto directo en el EspectroDeColores.
- Se han agregado etiquetas a las relaciones como "se forma en presencia de", "modifica angulo en", etc... Para detallar mejor cómo interactúan los componentes entre sí.
- Arcoiris ahora depende de la interacción con el Agua, ya que sin el agua no se formaría.
- EspectroDeColores tiene dependencia directa tanto de la reflexión como de la dispersión.

En cuanto a la cadena de suministros:
- Cada clase tiene ahora atributos adicionales como nombreProveedor, capacidadProduccion, nombreCliente, etc... Para dar más detalle.
- Se han añadido nuevas relaciones entre Distribuidor y Fabricante, y entre Minorista y Distribuidor, para reflejar pedidos y reposiciones de stock.
