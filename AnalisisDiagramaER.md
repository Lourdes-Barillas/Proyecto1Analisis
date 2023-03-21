# Generación de Diagrama de Entidad Relacion de Lavanderia
  Para la generacion de un diagrama primero se lee lo que solicita y durante el proceso se van anotando los nombres de las posibles tablas o elementos importantes que se necesitaran mas adelante. Las tablas principales son:
  
  * Usuarios
  * Clientes
  * Pedidos
  * Tipo Prendas(ropa)
  * Tipo Lavados
  * Precios
  * Insumos
  * Recetarios

  Ya teniendo las tablas o entidades principales empezamos a desglozarlas, escribiendo todos los atributos que contendra cada una de ellas; haciendo eso podemos ver que desglozaran otras tablas o tablas secundarias que se utilizaran para la union de las tablas principales evitando que incumplan con las normativas que impone el SQL en la generación de un diagrama o mas bien evitando las relaciones de n a n que son dificiles de relacionar, las tablas con sus tablas hijas son:
  
  * Usuarios
    * Roles
  * Clientes
    * Cliente_domicilios
  * Pedidos
    * Detalle_pedidos
  * Domicilios
    * Municipios
    * Cliente_domicilios
  * Tipo Prendas(ropa)
    * Colores
    * Tamaños(sizes)
  * Insumos
    * Marcas
    * Detalle_recetas
  * Recetarios
    * Detalle_recetas
 
  Sabiendo eso podemos empezar a unir o relacionar las tablas con sus debidas tablas hijas o dependencias de las mismas y prestando un poco de atención vemos hay tablas con mismas hijas lo cual significa que estamos evitando la relacion de n a n. Ya unificadas las tablas se empieza a unir todas las tablas por las cuales puedan tener o depender de otras tablas y asi obtendremos el diagrama final con el cual podremos ver el resultado final de como fluiran los datos.
  
  ![diagrama er lavanderia](https://user-images.githubusercontent.com/125481594/226219265-ed724787-664d-4211-add3-a2b07dbff82f.png)

