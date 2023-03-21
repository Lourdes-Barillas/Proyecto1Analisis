# Proyecto1Analisis
## REQUERIMIENTO SRS LAVANDERÍA<br>
### 1.1. INTRODUCCIÓN<br>
> En el presente documento se detalla los requerimientos de software y hardware 
> que se va a implementar en la lavandería para el correcto desarrollo y funcionamiento del sistema, 
> dentro de los parámetros establecidos en el enunciado del proyecto.  
### 1.2. PRÓPOSITO<br>
> La lavandería MasterClean necesita un sistema de logística de prendas que permita optimizar el 
> funcionamiento de sus operaciones y brindar a sus clientes tiempos de entrega más rápidos integrando 
> reportería que ayude a visualizar el estado de las prendas de una forma más eficiente, por lo que el 
> propósito de este documento es otorgar a los analistas, desarrolladores y stakhoulders un detalle 
> de los requerimientos que se implementarán, desde el alcance hasta las pantallas que integraran dicho sistema, 
> tomando en cuenta los lineamientos funcionales y no funcionales, así como también las restricciones 
> con el fin de llevar un control de calidad a lo largo del desarrollo y que sirva como una guía para los involucrados.  
### 1.3. ALCANCE<br>
> Dar una solución por medio de un sistema web a la lavandería MasterClean con el objetivo de optimizar los tiempos de 
> entrega y organizar el ingreso y egreso de prendas en dicha empresa, es un desarrollo que integra a la sucursal 
> ubicada en el centro comercial los Alamos, zona 4 San Miguel Petapa Guatemala que es la primera sede que abrió sus 
> operaciones en el año 2021.  
### 1.4. PERSPECTIVA DEL PRODUCTO<br>
> Este sistema será desarrollado para optimizar los tiempos de entrega y las operaciones de logística de la lavandería 
> por medio de una aplicación Web y así atraer a más personas para que utilicen el servicio de lavado, a los 
> administradores y empleados se las implementará interfaces intuitivas que cuenten con los protocolos de seguridad 
> de información para que cualquier operación que se realice sea almacenada en BDD´s.  
### 1.5. INTERFAZ DE USUARIO<br>
> La interfaz de los administradores y empleados debe ser minimalista para que sea de fácil aprendizaje al momento 
> de utilizarla, intuitiva y segura, debe contar con diferentes funciones separadas por módulos para que sea más 
> fácil la verificación de los usuarios, los estados de las prendas, la formas de pago y el ingreso a la reportería, 
> contar con método de seguridad extra de autenticación para que los administradores y empleados puedan ingresar de forma 
> segura y evitar robos de información al acceder a la página Web, debe contar con notificaciones que serán enviadas 
> en tiempo real a los clientes sobre el estado de sus prendas a su correo electrónico registrado o si lo prefieren 
> a su número de teléfono así como también alertas de cuándo estará cerrada la tienda, el personal y los clientes 
> deben sentir que cuentan con un asistente personal que controla el estado de las prendas.  
### 1.6. INTERFAZ DE SOFTWARE/HARDWARE<br>
> Al ser una página Web, se empleará un servidor para poder realizar las peticiones, una BDD y una comunicación 
> asincrónica para permitir que todos los empleados se puedan conectar al mismo tiempo y ejecutar diferentes tareas 
> sin afectar el funcionamiento general de la aplicación.  
>  - Servidor Web: será el encargado de gestionar la aplicación con todas las peticiones de los empleados y para el 
>  desarrollo del proyecto debe soportar .NET, Java, uno de los posibles candidatos es el servidor Heroku.  
>  - Base de Datos: será el banco de información de la aplicación, el cual almacenará la información de los usuarios 
>  y el estado de las prendas el servicio que se tiene contemplado para el desarrollo será MySQL.  
>  - Para nuestro proyecto, el back-up se realiza en un disco duro mecánico extraíble para mantener un método 
>  adicional a la nube como respaldo.  
> A coninuación se muestra la información que almacenará la BDD:  
>   1. ***Gestión de usuarios***: almacenará la información del personal y de los clientes.  
>       - Creación.  
>       - Modificación.  
>       - Bajas.  
>       - Bloqueos.  
>   2. ***Gestión de Órdenes***: almacena en la BDD el tipo de órden que ingresa al sistema.  
>       - Creación.  
>       - Modificación.  
>       - Eliminación.  
>   3. ***Gestión de estados para las órdenes***: llevar un control con el estado de las órdenes que ingresan al sistema.  
>       - Creación.  
>       - Modificación.  
>       - Eliminación.  
>   4. ***Gestión de Insumos***: llevar un inventario de los productos utilizados para el lavado.  
>       - Creación.  
>       - Modificación.  
>       - Eliminación.  
>       - Bloqueos.
>   5. ***Gestión de Proveedores***: llevar un control de los proveedores.  
>       - Creación.  
>       - Modificación.  
>       - Eliminación.  
>       - Bloqueos.  
>   6. ***Bitácora Consultas***: será una consulta general de todas las prendas y del listado de clientes.  
>       - Informe de Clientes.  
>       - Detalle de órdenes.  
>       - Descarte de prendas mayor a 90 días.  
>       - Inventario de Insumos.  
>       - Bitácora de Excepciones.    
>   7. ***Excepciones***: En todo sistema, se necesita de un control de excepciones para la mejora continua.  
>       - Gestión de empleados/usuarios.  
>       - Gestión de prendas.  
>       - Eliminaciones fallidas.  
>       - Cambio de estados fallidos.  
>       - Pagos fallidos.  
>       - Impresión de tikets fallidos.  
### 1.7. INTERFAZ DE USUARIO<br>
-	**Interfaz Principal**   
>   Él administrador y los empleados al ingresar a la página web tendrán una vista principal, donde deberá colocar su usuario y contraseña para ingresar al sistema, en caso de no contar con usuario o perder la contraseña, deberá solicitarle al administrador la creación de usuario o reinicio de contraseña.  
-	**Interfaz de Módulos**  
>   En esta pantalla el empleado tendrá una barra de herramientas en el perfil izquierdo de forma estática, el cual contará con los módulos siguientes:  
>   - Registro.  
>   - Ordenes.  
>   - Consultas.  
>   - Reportería.  
>   - Salida de la aplicación.  
-	**Módulo de Registro**  
>   En esta opción al empleado se le desplegará en la pantalla central un menú de sub-opciones que constará de las siguientes:  
>   - ***Registro Clientes***: el empleado podrá crear en esta opción a un cliente nuevo, ingresando los datos principales como DPI, NIT, Nombre y apellido, dirección y teléfono, el sistema creará un ID de cliente de forma automática.  
>   - ***Registro Insumos***: el empleado podrá crear en esta opción un nuevo insumo cuando no exista en el sistema, ingresando los datos principales como Nombre de Insumo y Proveedor, el sistema creará un ID automáticamente y se lo asignará al insumo.  
>   - ***Control de Inventarios***: el empleado al ingresar a esta opción podrá visualizar el inventario en tiempo real, con los siguientes ítems:  
>       - ID del insumo.  
>       - Nombre de insumo.  
>       - Disponibilidad.  
>       - Botón de consulta Detalle, donde podrá registrar entradas y salidas del mismo.  
-	**Módulo de Ordenes**  
>   En esta opción al empleado se le desplegará en la pantalla central un menú de sub-opciones que constará de las siguientes:  
>   - ***Ingreso de órdenes***: se desplegará otra pantalla para poder ingresar una orden nueva, se ingresará el número de DPI del cliente y al presionar el icono de lupa se filtrará, con este filtro se visualizará la información básica del mismo, Id cliente, nombre y un botón de ingreso de orden para poder registrar una orden nueva y generar un ticket impreso al cliente.  
>   - ***Cancelación de órdenes***: en esta opción se podrán cancelar órdenes, buscando con el número de orden.  
>   - ***Consulta de órdenes***: en esta opción, el usuario con el número de orden podrá consultar el estatus de la misma, los cuales serán:  
>       - Pendiente de Lavado.  
>       - Proceso de lavado.  
>       - Pendiente de Entrega al cliente.  
>       - Entregado al cliente.  
>       - Cancelado.  
>       - Desechado.  
-	**Módulo de Consultas**  
>   En esta opción al empleado se le desplegará en la pantalla central un menú de sub-opciones que constará de las siguientes:  
>   - ***Consulta de Clientes***: se visualizará en la pantalla principal el listado de clientes que se encuentran registrados, o se podrá buscar un cliente especifico con el número de DPI en el buscador de clientes, estos tendrán 2 opciones modificar o eliminar un registro.  
>   - ***Consulta de Insumos***: se visualizará en la pantalla principal el listado de insumos que se encuentran registrados, o se podrá buscar un insumo especifico con el ID en el buscador de insumos, este tendrá la opción de eliminar el registro.  
-	**Módulo de Reportería**  
>   En esta opción al empleado se le desplegará en la pantalla central un menú de sub-opciones que constará de las siguientes:  
>   - ***Informe de Clientes***: se exportará en un archivo .txt, la información general de los clientes registrados en el sistema:  
>       - ID cliente.  
>       - DPI.  
>       - NIT.  
>       - Nombre.  
>       - Dirección.  
>       - Teléfono.  
>   - ***Detalle de órdenes***: se exportará en un archivo .txt la información general de las ordenes ingresadas, con la opción de rango de fechas, la información a generar será:  
>       - No. Orden.  
>       - Detalle del cliente.  
>       - Detalle de prendas.  
>       - Total.  
>       - Fecha de Recepción.  
>       - Días en lavandería después de lavado.  
>       - Fecha de Entrega al cliente.  
>   - ***Descarte de prendas mayor a 90 días***: se exportará en un archivo .txt la información de la orden con las prendas a desechar.  
>       - No. Orden.  
>       - Nombre de cliente.  
>       - Fecha de Recepción.  
>       - Fecha de Descarte.  
>   - ***Inventario de Insumos***: se exportará en un archivo .txt la información del inventario de insumos, con la siguiente información:  
>       - Id insumo.  
>       - Nombre insumo.  
>       - Proveedor.  
>       - Cantidad existencia.  
>       - Se necesita pedido.  
>   - ***Bitácora de Excepciones***: se exportará en un archivo .txt la información del Excepciones, con la siguiente información:  
>       - Id Excepción.  
>       - Nombre Excepción.  
>       - Fecha de la Excepción.  
>       - Impacto de la Excepción (Alto, Medio, Bajo).  
### 1.8. FUNCIONES DE LAVANDERÍA MASTERCLEAN<br>
> La función de la lavandería es ofrecer a los clientes un servicio de lavado optimo, por lo que cuidar de las prendas y los productos que se utilizan pare este fin, es de suma importancia.  
>  1. Servicio a cualquier usuario que desee lavar sus prendas.  
>  2. Ingreso a cualquier empleado activo de la empresa a la página Web.  
>  3. Control de inventario.  
>  4. Recuperación de contraseña de usuarios fácil y seguro por medio de un administrador.  
>  5. Impresión de Ticket para el cliente.  
>  6. Envió de información por correo electrónico sobre status al cliente.  
>  7. Pago por medio de efectivo.  
>  8. Consulta de estados de prenda.  
>  9. Reportería general.  
### 1.9. REQUERIMIENTOS FUNCIONALES<br>
- **Gestión de Clientes**  
>  El sistema solo podrá brindar el servicio a clientes que se encuentren registrados asignándole un ID cliente, si no se encuentra dentro de la plataforma se deberá realizar el registro antes de recibir las prendas, se tendrá un control de los registros completo de todos los clientes con la finalidad de poder crear, modificar, eliminar o bloquear.  
- **Gestión de Empleados**  
>  El sistema solo podrá aceptar el ingreso a empleados que se encuentren registrados con un código, una contraseña y método de autenticación, si no se encuentra registrado, solo el administrador podrá realizar el registro y la contraseña, se tendrá un control de los registros completo de todos los empleados con la finalidad de poder crear, modificar, eliminar o bloquear cualquier empleado. 
- **Gestión de Insumos**  
>  El sistema llevará un inventario con la finalidad de tener un control de los insumos que se utilizan para el lavado de las prendas, se le asignará un código de insumo para catalogar los productos, si el insumo no esta registrado el empleado tendrá la opción de registrar, modificar o eliminar cualquier insumo.   
- **Gestión de Contraseñas**  
>  Como método de seguridad, el empleado solo podrá comunicarse con el administrador cuando pierda la contraseña asignada.  
- **Método de Autenticación**  
>  Como método de seguridad, el empleado solo podrá ingresar al sistema con un método de doble auntenticación, si necesita configurarlo debe llamar al administrador del sistema.  
- **Gestión de Consultas de estado**  
>  Para optimizar el tiempo de entrega se integra un control de estados con la finalidad de llevar el estado de cada prenda.  
- **Reportería**  
>  El sistema debe contar con un generador de reportes, para poder exportar información cuando se necesite, con la finalidad de ser aprovechada para futuros estudios de mercado o implementación de estrategias. Los reportes a generar serán los siguientes:  
>    - Informe de Clientes.  
>    - Detalle de órdenes.  
>    - Descarte de prendas mayor a 90 días.  
>    - Inventario de Insumos.  
>    - Bitácora de Excepciones.    
### 1.10. REQUERIMIENTOS NO FUNCIONALES<br>
- **Seguridad**  
>  El sistema podrá realizar validaciones de los usuarios y clientes que no se encuentren registrados en el sistema, adicional para los empleados tendrá un método doble de autenticación para poder ingresar a la plataforma. El protocolo de seguridad que se utilizará es HTTPS permitiendo una navegación confiable y segura para que pueda almacenar información o generar reportes sin ser vulnerado.  
- **Mantenimiento**  
>  El sistema debe contar con facilidad de mantenimiento a corto y largo plazo, será desarrollado por módulos con el fin de que cualquier requerimiento futuro que exista, pueda ser modificado sin problemas en su interfaz, código, servicios y BDD´s para no perder la integridad de los datos y las funcionalidades que ofrece el sistema, adicional que contará con manual de usuario.  
- **Confiabilidad**  
>  Para lograr la confiabilidad del sistema, debe ser cuidado cada una de las Excepciones que se produzcan en el mismo al momento de utilizar el sistema con el fin de detectar mejoras y solventar inconvenientes a la brevedad posible.  
- **Disponibilidad**  
>  El sistema debe estar disponible las 24 horas dependiendo el rol, para los administradores el uso del sistema no tendrá restricciones, para los empleados si tendrá un horario especifico empezando a las 6:00 a.m. y terminando a las 6:00 p.m., y será utilizado en cualquier navegador.  
- **Actualización**  
>  Se dará un constante monitoreo a las funcionalidades del sistema para mantenerlo actualizado frente a los diversas vulnerabilidades o errores que se produzcan.  
### 1.11. RESTRICCIONES<br>
>  1. Se manejará una restricción de ingreso al sistema por seguridad, empezando de 6:00 a.m. a 6:00 p.m. para los empleados.   
>  2. Se dará un máximo de 90 días para que el cliente pueda recoger su prenda, de lo contrario se desechará del sistema.   
>  3. No hay limitaciones de software, ya que se cuenta con los insumos necesarios para el desarrollo.  
>  4. Solo se utilizará aplicación Web.  
>  5. Solo se podrá trabajar en paralelo con conexión a MySQL Server.  
>  6. Este sistema debe ser auditable.  
>  7. No se permitirán otros protocolos que no estén contemplados en este documento TCP/IP, HTTPS. 
>  8. Solo se permitirá pagos en efectivo para poder retirar las prendas.  