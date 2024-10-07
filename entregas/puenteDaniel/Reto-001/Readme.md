##RETO-001 MODELOS DE DOMINIO ECO Y CADENA DE SUMINISTROS

#Introducción Eco
Este proyecto modela un sistema que simula la transmisión, reflexión y captura de sonido. Se basa en un conjunto de clases y objetos interrelacionados que representan el comportamiento de una fuente de sonido (como una persona), un medio (como el aire), una superficie reflexiva (como una pared de hormigón), y un receptor (como un micrófono).

#Clases Principales
FuenteSonora: Representa la fuente emisora del sonido, como un altavoz.
Sonido: Modela el sonido y sus propiedades  mientras viaja por el medio.
Medio: El medio por el cual viaja el sonido, como el aire.
SuperficieReflexiva: Superficie que refleja el sonido, como una pared.
Receptor: Dispositivo que recibe el sonido reflejado, como un micrófono.

#Introducción Cadena de Suministros
Es un sistema que abarca todas las actividades relacionadas con la creación, almacenamiento y distribución de productos desde el proveedor hasta el cliente final. Este modelo ayuda a entender cómo se gestionan las relaciones entre diferentes entidades involucradas en el proceso.

#Clases Principales
Proveedor: Encargado de suministrar productos a los almacenes. Puede tener múltiples tipos de productos.
Almacén: Almacena temporalmente los productos antes de su distribución. Maneja el inventario disponible.
Transportista: Responsable del transporte de productos desde el almacén hasta el cliente. Debe tener en cuenta su capacidad de carga.
Cliente: Destinatario final de los productos, quien realiza el pedido y recibe la entrega.
