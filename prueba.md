# Documentar las pruebas

### DESCRIPCIÓN DEL PROYECTO
La lavanderia es una empresa que se dedica a ofrecer servicios de lavado y secado de ropa de sus clientes. El objetivo de este proyecto es documentar las pruebas que se han realizado en una aplicación web de la lavandería, con el fin de asegurar su correcto funcionamiento.

### Alcance
Este documento se enfoca en las pruebas realizadas en la lavandería, que incluye las siguientes áreas:
  * Recepción de la ropa sucia
  * Lavado y Secado de la ropa
  * Doblado y empaquetado de la ropa
  * Entrega de la ropa

### Pruebas
Recepción de la ropa sucia
 * Prueba 1: Verificación de que se registra la información del cliente correctamente
   * Descripción: Se ingresa información del cliente en el sistema, incluyendo nombre, número de teléfono y tipo de servicio solicitado.
   * Resultado esperado: La información del cliente se registra correctamente en el sistema y se muestra en la pantalla de empleado de recepción.
 * Prueba 2: Verificación de que se pesa la ropa adecuadamente
   * Descripción: Se pesa la ropa en la balanza y se ingresa el peso en el sistema.
   * Resultado esperado: El peso de la ropa se registra correctamente en el sistema y se muestra en la pantalla del empleado de recepción.

### Lavado y Secado de la Ropa
 * Prueba 1: Verificación que la ropa se lava con el detergente adecuado
   * Descripción: Se verifica que se use el detergente adecuado para cada tipo de ropa.
   * Resultado esperado: Se muestra en la pantalla del empleado encargado del lavado.
* Prueba 2: Verificación de que la ropa se seca a la temperatura adecuada
  * Descripción: Se verifica que se use la temperatura adecuada para cada tipo de ropa.
  * Resultado esperado: Se muestra en la pantalla del empleado encargado del secado.

### Doblado y Empaquetado de la ropa
* Prueba 1: Verificación de que la ropa se dobla correctamente
  * Descripción: Se verifica que la ropa se dobla segun el tipo de prenda.
  * Resultado esperado: Se muestra en la pantalla del empleado encargado del doblado.
* Prueba 2: Verificación de que la ropa se empaqueta adecuadamente
  * Descripción: Se verifica que la ropa se empaqueta adecuadamente según el tipo de prenda.
  * Resultado esperado: Se muestra en la pantalla del empleado encargado del empaquetado.

### Pago Efectivo
* Prueba 1: Pago del cliente al empleado encargado de la lavanderia
  * Descripción: Se le recibirá al cliente el pago unicamente en efectivo
  * Resultado esperado: Se muestra en la pantalla del empleado encargado del efectivo recibo.

### Tiempo de Prenda en la Tienda
* Prueba 1: La lavanderia solo se hará cargo de 2 días máximo de la prenda despues de esos 2 días pasará hacer pertenecia de la lavandería.
  * Descripción: Se tendrá la prenda en la lavanderia 2 días no más.
  * Resultado Esperado: Se muestra en la pantalla del empleado encargado si recogieron la prenda en el tiempo estimado o no. 

### Entrega de la Ropa Limpia
* Prueba 1: Verificación de que se entrega la ropa limpia a tiempo
  * Descripción: Se verifica que la ropa se entrega en el plazo acordado con el cliente.
  * Resultado esperado: La ropa se entrega en el plazo acordado con el cliente.


# Documentar la implementación
Este proyecto tiene como objetivo implementar una aplicación web para la gestión de una lavandería. La aplicación permitirá a los usuarios realizar pedidos de lavado y planchado de ropa y al personal de la lavandería gestionar dichos pedidos.

### Requisitos
Para poder ejecutar este proyecto en su equipo local, necesitará tener instalado lo siguiente:

### Uso
Para utilizar la aplicación, puede registrarse como usuario o ingresar como personal de lavandería.

### Encargado de Tienda
Como encargado de la tienda, puedes gestionar los pedidos de los usuarios. Para hacerlo, sigue estos pasos:
1. Ingresa a la aplicación en tu navegador web en la dirección
2. Haz clic en el botón "Iniciar sesión" y completa el formulario de inicio de sesión con las credenciales de un usuario con rol de personal de la lavandería.
3. Haz clic en el botón "Pedidos"
4. Verás una lista para registrar o buscar clientes y para gestionar productos de lavandería, consulta BDD prendas o reporteria de prendas olvidadas o entregadas
5. Cuando hayas escogido una opción de la lista, haz clic en el botón "Siguiente"
6. Cuando hayas completado el pedido, haz clic en el botón "Completar pedido".

### Contribuciones
Si deseas contribuir a este proyecto, por favor sigue estos pasos:
1. Realiza un fork de este repositorio
2. Crea una nueva rama para tus cambios
3. Realiza los cambios en tu rama
4. Haz commit de tus cambios
5. Sube tus cambios a tu fork
6. Crea un pull request para que tus cambios sean considerados para la rama principal de este repositorio.
