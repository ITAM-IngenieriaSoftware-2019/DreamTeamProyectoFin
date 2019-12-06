# Software Requirements Specification
## For RappITAM

#### Prepared by: 
+ Cecilia Vásquez Perez- 150482 
+ Diego Villalvazo Sulzer - 155844 
+ Ana Carolina Sandoval Mejía - 152808
+ Stephanie Lizeth Malvaes Diaz -135515

#### DreamTeam
06 de diciembre de 2019

# Tabla de contenidos
1. **Introducción**  
   1.  Propósito Convención.
   2.  Audiencia. 
   3.  Alcance del producto.
   4.  Referencias. 
2. **Drescripción**  
   1. Perspectiva del producto
   2. Funciones del producto
   3. Clases y caracteristicas
   4. Ambiente de operación
   5. Limitaciones del diseño e implementación
   6. Documentación
   7. Dependencias y supuestos
3. **Requerimientos Externos**
   1. Interfaces de Usuario.
   2. Interfaces de Hardware. 
   3. Interfaces de Software.
   4. Interfaces de comunicación
4. **Funcionalidad del sistema**
   1. 
   2. 
   3. 
5. **Requerimientos no funcionales**
   1. Requerimientos de rendimiento
   2. Requerimientos de seguridad
   3. Requerimientos de fiabilidad

   # 1. Introducción
      ## 1.1 Propósito
      El propósito de este documento es proporcionar una descripción detallada de los requisitos para una aplicación que funciona como un sistema de delivery para los alumnos del ITAM llamada **RappITAM**, también se explicarán las limitaciones del sistema y su interfaz.
   
      ## 1.2 Audiencia
      La audiencia de este documento son los desarrolladores del proyecto (equipo DreamTeam), la supervisora del proyecto (Paulina Bustos) y posiblemente los usuarios finales. Los usuarios finales incluyen alumnos del ITAM que pueden fungir como clientes o repartidores. Se recomienda al lector leer el documento en orden y, dependiendo del tipo de audiencia, se recomienda enfocarse en las secciones pertinentes al uso que el lector dará a la aplicación.

      ## 1.3 Alcance del producto
      El sistema RappITAM es un software para que alumnos del ITAM puedan realizar pedidos a los  diferentes establecimientos alrededor de la escuela, esto con la finalidad de optimizar sus horas de estudio sin descuidar su alimentación o salud. 
      Los alumnos podrán realizar pedidos de 3 categorias: restaurantes, cafeterias y farmacias. Además, la aplicación tiene una sección de _favoritos_ en donde se guardan los lugares a los que el usuario más realiza pedidos esto es con el fin de optimizar el tiempo que pase dentro de la aplicación y pueda seguir con sus activides. La aplicación también tiene la sección _búsquedas recientes_ en donde se mostrarán los últimos restaurantes/tiendas que buscó el alumno.
      
   
   ## 1.4 Referencias


   # 2. Descripción General
   
   ## 2.1 Perspectiva del producto
   Esta aplicación forma parte de un proyecto de la materia Ingeniería de Software.El cual cumple con una funcionalidad similar a la de otras aplicaciones como _Rappi, UberEats, sin delantal, etc._ Pero con la diferencia de que esta aplicación es únicamente para alumnos del ITAM,los productos serán entregados en las instalaciones del ITAM y los negocios participantes son aquellos que esten en las cercanias de la institución.
 
   ## 2.2 Funciones del producto
   Las funcionalidades principales del producto son las siguientes:
 
   - Registro      
   - Inicio de sesion    
   - Búsqueda
   - Favoritos   
   - Establecimiento   
   - Carrito
   - Checkout
         
   ## 2.3 Clases de Usuarios y caracteristicas
   
   - **Usuario principal**
      
      Los alumnos del ITAM conformaran a los usuarios principales de la aplicacion. Estos usuarios hacen uso de la aplicacion para pedir comida y otros productos de establecimientos cercanos al ITAM. Para esto, los alumnos se registran y hacen sesion en la aplicacion.
   
   - **Repartidor**
   
      Los alumnos del ITAM tambien pueden fungir como repartidores para la aplicacion, ellos reciben los pedidos que otros alumnos hacen y van al establecimiento para recoger el pedido y, posteriormente, entregan el pedido al alumno en el lugar definido por el usuario principal y cobran el total del pedido en caso de que se haya elegido la opcion de pagar con efectivo.
   
   ## 2.4 Ambiente operacional
   
      Este sistema esta diseñado como una aplicacion para telefonos inteligentes, la cual podra ser descargada desde las tiendas como _Apple Store, Google Play_, etcétera. La aplicacion tendra actualizaciones las cuales estaran disponibles para descargar en las tiendas de aplicaciones; estas actualizaciones seran para realizar mejoras y posiblemente para mejorar bugs. Esta es una aplicacion _standalone_, es decir no depende ni convive con otras aplicaciones en el mercado. Se eligio usar una plataforma movil, pues es la forma mas facil y rapida para hacer pedidos, además de ser la más popular.
   
   ## 2.5 Limitaciones de diseño e implementación
   
      La limitación principal de esta aplicación es que solamente los alumnos del ITAM pueden hacer uso de esta aplicación, incluso no podría ser usada por profesores ni trabajadores del ITAM pues esto podría suponer problemas ya que los repartidores de la aplicación son solamente alumnos, lo cual es otra limitación. Limitaciones de hardware como tiempo y memoria no son un problema aquí pues este tipo de aplicaciones no ocupa muchos recursos en los teléfonos inteligentes.
 
   ## 2.6 Documentación de usuario

      En este caso no consideramos necesario un manual para los usuarios pues este tipo de aplicaciones son intuitivas y fáciles de usar, además de que esta aplicación funciona muy similarmente a otras en el mercado. Por otro lado, sí consideramos que es necesario un pequeño tutorial que se despliegue al iniciar sesión en la aplicacion por primera vez, en donde se explique brevemente cómo usar las funcionalidades principales.

   ## 2.7 Dependencias y supuestos
      Se asume que los usuarios cuentan con un teléfono inteligente en condiciones optimas con los funcionamientos básicos y acceso a internet, esto es necesario para poder descargar la aplicación. 

   # 3. Requerimientos Externos
   ## 3.1. Interfaces de Usuario.
      
      Cada interfaz grafica en la aplicacion corresponde a una funcionalidad, como la descrita en la seccion _Funcionalidades del Sistema_. Referirse al prototipo para ver las interfaces de usuario.

   ## 3.2 Interfaces de Hardware
  
      Los dispositivos que soportan esta aplicación son teléfonos inteligentes relativamente nuevos (de no más de 10 años) con acceso a internet y que tengan acceso a una tienda de aplicaciones como _Apple Store_ o _Google Play_. Los datos utilizados, que están guardados en una base de datos, son tanto categóricos, como numéricos. Los datos categóricos son nombre del alumno, correo electrónico, usuario, nombre del establecimiento, nombre del producto, estatus del establecimiento (abierto o cerrado) y estatus del producto (disponible o agotado), todos estos son nominales. Los datos numéricos son número telefónico del usuario.
  
   ## 3.3 Interfaces de software
      
      Esta aplicación se conecta con una base de datos que contiene los datos de los usuarios, los repartidores, los establecimientos y sus productos. Esta aplicación estará disponible en iOS y Android para su primera versión. Los datos o mensajes de entrada son las peticiones de los usuarios y las actualizaciones de los productos en los establecimientos, los datos o mensajes de salida son las confirmaciones de los pedidos.
      
   ## 3.4 Interfaces de comunicación
      
      La aplicacion se comunica con la base de datos que se encuentra en un servidor y viceversa por medio de Internet con ayuda del protocolo HTTP. A la vez, la base de datos se comunica mediante el protocolo SMTP para enviar correos a los alumnos con la confirmación de sus pedidos. Los datos solamente pueden ser accesados si el alumno o usuario introduce introduce las credenciales correctas para así garantizar la seguridad del sistema. Además, los datos enviados mediante los protocolos de Internet son todos encriptados para evitar robo de información. Finalmente, el sistema es resistente a ataques DoS.
      
      # 4. **Funcionalidad del sistema**
      
    
    ## 4.1 Registro
    
    ### Descripción y prioridad
      En esta sección el usuario se registra en la aplicacion cuando todavia no ha creado una cuenta. Para esto, se le pide al usuario que ingrese los siguientes datos: Nombre completo, numero telefonico, correo electronico, usuario, contraseña y confirmacion de la contraseña. Esta funcionalidad tiene prioridad media, pues por medio de esta se garantiza la identidad de los usuarios y, así, la seguridad de los alumnos.
      
    ### Secuencias de estímulo/respuesta
      Esta es la segunda pantalla que se muestra, después de la de inicio de sesión. Si el usuario no se ha registrado, la pantalla de inicio de sesión lleva a la de registro. Después de hacer el registro, se envía un correo al alumno para confirmar su cuenta.
      
    ### Requerimientos Funcionales
    1. El correo electrónico debe terminar en _@itam.mx_ para garantizar que el alumno estudia efectivamente en el ITAM.
    2. El numero telefonico debe ser a 10 digitos
    3. El nombre del usuario no debe tener numeros o caracteres especiales
    4. La contraseña debe ser de al menos 8 caracteres, con mayusculas, minusculas y un numero o caracter especial.
      
    ## 4.2 Inicio de sesion
    
    ### Descripción y prioridad
      El usuario ingresa a esta sección para poder hacer uso de la aplicacion. Aqui, el usuario ingresa su usuario, contraseña y oprime el boton _Iniciar sesion_ para poder ingresar a su cuenta dentro de la aplicacion. Esta funcionalidad tiene prioridad baja.
   
    ### Secuencias de estímulo/respuesta
    Esta es la primera pantalla que se muestra al usuario cuando descarga la aplicacion por primera vez o si tiene la sesion cerrada.
    
    ### Requerimientos Funcionales
    1. El nombre de usuario debe haber sido registrado exitosamente
    2. El usuario debe haber confirmado el correo que le llego con su registro para poder iniciar sesion por primera vez
    3. El nombre de usuario y la contraseña deben ser correspondientes a las que el alumnos registro.
    
    ## 4.3 Búsqueda
    
    ### Descripción y prioridad
      En esta sección hay una barra de texto en donde el alumno escribe el nombre del establecimiento o el tipo de productos que busca (desayunos, vegana, medicamentos) y al hacer la búsqueda, aparece una lista con los establecimientos.
      Otra forma de buscar, es por restaurantes o tiendas. Al apretar el botón _restaurantes_, aparecerá en la aplicación una lista de ellos ordenada por popularidad. Análogamente, aparecerán tiendas al apretar el botón _Otras tiendas_. Esta funcionalidad tiene prioridad alta, pues con este motor de búsqueda el usuario encuentra los establecimientos en donde hará los pedidos, además se debe garantizar que la búsqueda sea amigable para los usuarios y eficiente.
      
    ### Secuencias de estímulo/respuesta
    Esta es la primera pantalla que se muestra una vez que el usuario inicio sesion exitosamente. Esta pantalla tambien se muestra cuando se presiona el boton _Buscar_ en la barra de navegacion.
    
    ### Requerimientos Funcionales
    1. Los establecimientos mostrados deben estar en horario de operaciones.
    2. Los establecimientos mostrados deben estar abiertos (no cerrados o clausurados).
    3. Los establecimientos mostrados deben estar a un kilometro a la redonda del ITAM.
     
    ## 4.4 Favoritos
   
    ### Descripción y prioridad
      En esta sección se muestran los restaurantes/tiendas favoritas del usuario para que así el usuario pueda acceder más fácilmente a los establecimientos que más le gustan y en donde más realiza pedidos. Cuando el usuario no ha hecho ninguna búsqueda ni compra, en esta seccion aparecen los establecimientos más populares. Esta funcionalidad tiene prioridad baja, pues si bien ayuda a optimizar los tiempos de búsqueda y a mejorar la experiencia de usuario, no es una funcionalidad necesaria para poder hacer pedidos.
    
    ### Secuencias de estímulo/respuesta
    Esta pantalla  se muestra cuando se presiona el boton _Favoritos_ en la barra de navegacion.
    
    ### Requerimientos Funcionales
    1. Los establecimientos que aparecen aqui deben ser aquellos que hayan sido seleccionados como favoritos.
   
    ## 4.5 Establecimiento
   
    ### Descripción y prioridad
      Se accede a esta sección al seleccionar un establecimiento, en esta se muestra la lista de productos que ofrece dicho lugar. Al seleccionar un producto, éste se agrega al carrito de compras y el usuario puede seguir viendo la lista de productos. Esta funcionalidad tiene prioridad alta pues cada pedido contiene productos de un establecimiento y es necesario que el usuario tenga visibilidad de los productos para poder hacer pedidos.
      
    ### Secuencias de estímulo/respuesta
    Se accede a un establecimiento de varias formas: en la seccion _Busqueda_ donde aparecen los establecimientos mas populares, al hacer una busqueda en _Busqueda_ y en la seccion _Favoritos_
    
    ### Requerimientos Funcionales
    1. El establecimiento debe estar abierto (no cerrado o clausurado).
    2. El establecimiento debe estar a un kilometro a la redonda del ITAM.
    3. Los productos mostrados deben estar disponibles.
   
    ## 4.6 Carrito
   
    ### Descripción y prioridad
      En esta sección se muestran los productos que se agregaron de un establecimiento determinado. Aqui se puede modificar las cantidades de los productos seleccionados (añadir o eliminar) y se puede eliminar un producto por completo del carrito. Ademas en esta seccion se muestra el subtotal de todos los productos para que el usuario vea el total de su pedido. También se muestra la direccion de entrega del pedido, la cual se puede modificar dentro de esa sección.Al presionar el boton "Continuar", el usuario es llevado a la seccion _Checkout_. Esta funcionalidad tiene prioridad media pues el carrito es necesario para que el usuario pueda hacer un pedido.
      
    ### Secuencias de estímulo/respuesta
    Se ingresa al carrito al apretar el boton en forma de carrito de compras dentro de cada establecimiento.
    
    ### Requerimientos Funcionales
    1. Los productos deben mostrar los precios actualizados.
    2. El pretotal mostrado debe concidir con la suma de los precios de todos los articulos en el carrito
      
    ## 4.7 Checkout
   
    ### Descripción y prioridad
       En esta interfaz se muestra la direccion (salon o lugar del ITAM) a la cual sera entregada el pedido, el metodo de pago seleccionado; estas dos variables pueden ser cambiadas por el usuario al seleccionar el boton _Cambiar_. Esta seccion tambien tiene la opcion de agregar un cupon y de dividir la cuenta. La ultima feature de esta seccion es un resumen del total de pago, dividido en costo de productos y costo de envios. Finalmente, al seleccionar el boton _Enviar pedido_, el pedido se crea y se le cobra el total al alumno. Esta funcionalidad tiene prioridad alta pues el checkout es necesario para que el usuario pueda hacer un pedido.
     
    ### Secuencias de estímulo/respuesta
    Se ingresa a esta seccion despues de seleccionar el boton _Continuar_ en el Carrito.
    
    ### Requerimientos Funcionales
    1. El total mostrado debe ser igual a la suma del total de los productos mas el costo de envio.
    2. Si el pago sera con tarjeta, se debe garantizar que la tarjeta sea valida y que procedio el pago antes de confirmar el pedido.
    

# 5. Requerimientos no funcionales
   ## 5.1 Requerimientos de rendimiento

   El sistema debe garantizar que el registro tome menos de 10 segundos y que el inicio de sesión tome menos de 5 segundos. El sistema también debe garantizar que los pedidos tomarán menos de 10 segundos en ser registrados y confirmados.

   ## 5.2 Requerimientos de fiabilidad
   
   Para seguridad de los alumnos, se deben tener filtros para garantizar que los repartidores y los usuarios sean solamente alumnos del ITAM. Además, la foto y nombre del repartidor debe ser visible para el usuario y viceversa.
   
   ## 5.3 Requerimientos de seguridad
   
   - El sistema debe ser resistente a ataques, por ejemplo, D-DOS. Para así garantizar fiabilidad y rendimiento al usuario.
   - El sistema debe cuidar la confidencialidad de los usuarios y la integridad de los datos, esto se puede hacer mediante la encriptación de los datos enviados y recibidos por el sistema.
  
   ## 5.4 Atributos de calidad del software
- El sistema debe garantizar tener pocos incidentes de alta prioridad, por ejemplo, teniendo un sistema alterno que sirva como DR (Disaster Recovery) en caso de algún problema.
- El sistema debe garantizar ser resistente a un fuerte uso del sistema, por ejemplo, a la hora de la comida.
