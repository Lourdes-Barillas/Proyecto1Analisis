## Diseño de la aplicación para los servicios de una lavandería
> El análisis de esta aplicación se ha discutido con los integrantes del proyecto y se ha realizado un análisis a sus aportes y como primer fase de documentación, en este documento damos a entender el diseño hasta ahora idealizado por los participanes.
### 3.1 Desarrollo del problema<br>
#### Problema
>> El problema a solucionar contiene las siguientes determinantes:
>>> 1. La gestión de usuarios que solicitan servicios
>>> 2. La gestión de insumos
>>> 3. La gestión de ventas
>>> 4. Atracción al público
#### Solución al problema
>> El programa tiene las siguientes características que resuelven los problemas principales
>>> 1. El usuario es registrado para un requerimiento futuro de la lavandería
>>> 2. El usuario visualiza su prenda en proceso en tiempo real
>>> 3. Los insumos son registrados al momento de detectar su entrada y brinda el aviso si estamos a punto de quedarnos sin provisiones para pedir más
>>> 4. La ventas serán ahora guardadas en una base de datos
>>> 5. Se planea esta interacción con el cliente desde el sitio web y de esta manera, que ellos se sientan atraídos a los servicios de la lavandería y quieran saber el estado de sus prendas y preferir a esta compañía.
### 3.2 Diseño de las pantallas y su utilidad
#### Autenticación
>>> 1. Autenticación del encargado de la lavandería
>>> 2. Autenticación del cliente en su dispositivo
>>> 3. Autenticación de administradores de insumos
>>> 4. Autenticación de administradores y gerentes
#### Consulta de clientes
>>> 1. Pantalla que consulte a un cliente para registrar el ticket solicitando el servicio de lavado
>>> Para este requerimiento se necesita una base de datos que consulte al cliente y tenga las restricciones necesarias en las que sólo el cliente puede saber su password y el encargado de la tienda pueda asistirle desde el sistema accediendo a su código, nombre y apellido, número de teléfono, correo y otras limitantes.
>>> 2. Pantalla para agregar a un cliente si no existe (Esto no incluye crear una cuenta en línea para ahorrar el espacio de datos que sólo cuentas en línea guardan y dejar esta decisión al cliente por si no quieren tenerla
### Gestión de productos
>>> Debe existir un apartado para la gestión de productos. Todo esto es discutible con el stakeholder. Se pueden introducir varias pantallas o una por cada requerimiento si son necesarios o aceptados por el cliente, determinando las siguientes funciones.
>>> 1. Gestionar los proveedores para obtener descuentos al obtener un mayor cantidad de productos
>>> 2. Gestionar entrada de productos
>>> 3. Gestionar necesidad de productos
### Agregar la prenda a un proceso de servicio de lavado
>>> Se deben analizar las condiciones de la prenda en una pantalla administrada por el encargado de la lavandería en donde se utilicen las siguientes funciones
>>> 1. Anotar las caraterísticas de la prenda como deficiencias de tela, color de la tela, falta de elementos como el botón de una camisa, etc.
>>> 2. Seleccionar el tipo de servicio requerido para un cuidado adecuado de la tela
>>> 3. Según el tipo de servicio, indicar la cantidad de tiempo que esta requerirá
>>> 4. Después de tener la prenda lista, ponerla en la cola de entrega por 90 días.
### Implementación de un sitio web para el usuario para tener conocimiento del proceso que lleva su tela y revisar en cuánto puede ir por ella
>>>Este sitio web es discutible con el cliente si lo necesita o no. Esto es idea del equipo que procesa el desarrollo de la aplicación y si el cliente lo acepta, lo implementamos. Esto queda al pendiente de una respuesta del cliente.
#### Características principales del sitio
>>> 1. Login del cliente
>>> 2. Ver en tiempo real el proceso de su prenda
