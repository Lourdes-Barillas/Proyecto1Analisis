# Proyecto1Analisis
**REQUERIMIENTO SRS LAVANDERÍA**
    **1.1.INTRODUCCIÓN**
        En el presente documento se detalla los requerimientos de software y hardware 
        que se va a implementar en la lavandería para el correcto desarrollo y funcionamiento del sistema, 
        dentro de los parámetros establecidos en el enunciado del proyecto.  
    **1.2.PRÓPOSITO**
        La lavandería MasterClean necesita un sistema de logística de prendas que permita optimizar el 
        funcionamiento de sus operaciones y brindar a sus clientes tiempos de entrega más rápidos integrando 
        reportería que ayude a visualizar el estado de las prendas de una forma más eficiente, por lo que el 
        propósito de este documento es otorgar a los analistas, desarrolladores y stakhoulders un detalle 
        de los requerimientos que se implementarán, desde el alcance hasta las pantallas que integraran dicho sistema,
        tomando en cuenta los lineamientos funcionales y no funcionales, así como también las restricciones 
        con el fin de llevar un control de calidad a lo largo del desarrollo y que sirva como una guía para los involucrados.  
    **1.3.ALCANCE**
        Dar una solución por medio de un sistema web a la lavandería MasterClean con el objetivo de optimizar los tiempos de 
        entrega y organizar el ingreso y egreso de prendas en dicha empresa, es un desarrollo que integra a la sucursal 
        ubicada en el centro comercial los Alamos, zona 4 San Miguel Petapa Guatemala que es la primera sede que abrió sus 
        operaciones en el año 2021.
    **1.4.PERSPECTIVA DEL PRODUCTO**
        Este sistema será desarrollado para optimizar los tiempos de entrega y las operaciones de logística de la lavandería 
        por medio de una aplicación Web y así atraer a más personas para que utilicen el servicio de lavado, a los 
        administradores y empleados se las implementará interfaces intuitivas que cuenten con los protocolos de seguridad 
        de información para que cualquier operación que se realice sea almacenada en BDD´s.
    **1.5.INTERFAZ DE USUARIO**
        La interfaz de los administradores y empleados debe ser minimalista para que sea de fácil aprendizaje al momento 
        de utilizarla, intuitiva y segura, debe contar con diferentes funciones separadas por módulos para que sea más 
        fácil la verificación de los usuarios, los estados de las prendas, la formas de pago y el ingreso a la reportería, 
        contar con método de seguridad extra de autenticación para que los administradores y empleados puedan ingresar de forma 
        segura y evitar robos de información al acceder a la página Web, debe contar con notificaciones que serán enviadas 
        en tiempo real a los clientes sobre el estado de sus prendas a su correo electrónico registrado o si lo prefieren 
        a su número de teléfono así como también alertas de cuándo estará cerrada la tienda, el personal y los clientes 
        deben sentir que cuentan con un asistente personal que controla el estado de las prendas. 
    **1.6.INTERFAZ DE SOFTWARE/HARDWARE**
        Al ser una página Web, se empleará un servidor para poder realizar las peticiones, una BDD y una comunicación 
        asincrónica para permitir que todos los empleados se puedan conectar al mismo tiempo y ejecutar diferentes tareas 
        sin afectar el funcionamiento general de la aplicación.
            - Servidor Web: será el encargado de gestionar la aplicación con todas las peticiones de los empleados y para el 
                            desarrollo del proyecto debe soportar .NET, Java, uno de los posibles candidatos es el servidor Heroku.
            - Base de Datos: será el banco de información de la aplicación, el cual almacenará la información de los usuarios 
                            y el estado de las prendas el servicio que se tiene contemplado para el desarrollo será MySQL.
            - Para nuestro proyecto, el back-up se realiza en un disco duro mecánico extraíble para mantener un método 
                            adicional a la nube como respaldo.
        A coninuación se muestra la información que almacenará la BDD:
            1.  **Gestión de usuarios**: almacenará la información del personal y de los clientes.
                    	Creación.
                    	Modificación.
                    	Bajas.
                    	Bloqueos.     
            2. **Gestión de Prendas**: almacena en la BDD el tipo de prenda que ingresa al sistema.
                    	Creación.
                    	Modificación.
                    	Eliminación.


    
    1.7.

    