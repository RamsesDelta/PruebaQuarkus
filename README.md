Problemas:

1 Conocer el framework quarkus
Solucion: Leer la documentacion que ofrece quarkus, asi como tambien foros, y hacer ejemplos

2 No poder conectarme a la BD de MySQL, ya que al compilar el proyecto marcaba error que el puerto ya estaba ocupado
Solucion: agrege la siguiente linea -Ddebug=1234 para que cambiara el puerto 

3 Consumir otro servico de Compñias desde el servicio de Productos, con la finalidad de llamr un metodo de compañias que me permita saber si existe
Solucion: me base en la documentacion, el cual sugerian crear un interface usando la anotacion @RegisterRestClient

4 Cambiar los nombres de las variables de instancia de la entidad de Productos
Solucion: investige por lo que la sulucion era poner la anotacion @JsonbProperty para que se cambie el nombre en el JSON

5 Actulizar un registro de OneToMany a ManyToOne (no solucione de actulizacion al agregar un registro nuevo de variantes)
Solucion: para hacer la actulizacion de Productos y Variantes, en el caso de productos solo use un metodo find mapie los campos, pero en
caso de Variantes tuve que hacer un forEach y dentro del forEach use un findById y mapie los campos
