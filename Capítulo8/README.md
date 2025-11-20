# Proyecto final

## Objetivos
Al finalizar la práctica, serás capaz de:
- Conectar orígenes de datos.
- Realizar transformaciones.
- Crear vistas.
- Diseñar dashboards.


## Objetivo visual 

<img src="../images/08/00.png" width="500" >



## Duración aproximada
- 120 minutos.


## Instrucciones 

### Tarea 1. Conexión y preparación de datos
1.	Para este primer ejercicio, descarga el material de la carpeta Primer Proyecto / Data, que ya tienes disponible en el material proporcionado.
2.	Analiza la data proporcionada y realiza una primera inspección para la limpieza de datos.


<img src="../images/08/01.png"  >
<img src="../images/08/02.png"  >
<img src="../images/08/03.png"  >

### Tarea 2. Limpieza de datos

Desarrolla un dashboard que permita analizar la cantidad de toneladas de fruta exportadas a clientes de distintos países.

Requerimientos:
•	Cantidad de toneladas por cliente.
•	Cantidad de toneladas por empresa.
•	Cantidad de toneladas de clientes por fruta.
•	Ganancias de exportación por país.
•	% de las ganancias por país respecto al monto total.
•	% de las exportaciones en toneladas por país.


<img src="../images/08/04.png"  >


Organiza la data creando una carpeta en tu equipo para estructurar los archivos. 

<img src="../images/08/05.png"  >

Luego, conecta los distintos archivos en Tableau.

- Abre Tableau Desktop, ve a la primera pantalla junto donde aparece `CONECTAR`.

<img src="../images/08/06.jpg"  >

- Conecta el archivo Excel Data Exportaciones.

<img src="../images/08/07.jpg"  >

- Arrastra `DATA EXPORTACIONES` y, posteriormente, `CLIENTES`.

<img src="../images/08/08.jpg"  >


•	Conecta el archivo TXT FRUTAS.

<img src="../images/08/09.jpg"  >

Ya que seleccionaste el tipo de data como texto, selecciona el texto formateado de `FRUTAS` dando clic en `Abrir`.

<img src="../images/08/10.jpg"  >


Realiza el mismo proceso que realizaste con la data de Excel, arrastra a la paleta de trabajo y observa que, en automátic,o de nuevo crea esta relación de información

<img src="../images/08/11.jpg"  >

Une la última data el CSV de nombre Empresas al proyecto en Tableau.

<img src="../images/08/12.jpg"  >


Haz clic sobre `Data CSV`, selecciona la carpeta `Empresas` y da clic sobre el archivo `Empresas`.

<img src="../images/08/13.jpg"  >

Crea esta conexión de datos, arrastra el archivo y observa qué sucede. Debes  enlazar este archivo directo al archivo principal.

<img src="../images/08/14.jpg"  >

Presenta un error al realizar la relación, no identifica qué campos unir. De aquí la importancia de conocer la data con la que se trabajará, para brindar una estructura correcta en esta primera fase y porque es el cimiento del Dashboard

¿Cómo solucionarlo? Es sencillo:  une la data de ambos archivos con el campo ID `Empresas`.

<img src="../images/08/15.jpg"  >

Luego que ya tienes las conexiones en las diferentes conexiones de datos, llegó el momento de realizar la visualización de datos. Lo primero es  aplicar un filtro a nivel ` Origen `.

Ve a la pestaña de `Hoja1` y selecciona los datos `DATA EXPORTACION ` selecciona el cambio `CANTIDAD EN KG`. 

<img src="../images/08/16.jpg"  >

Ya que estás en la pestaña de fuente de datos, da clic en `añadir filtros`.

<img src="../images/08/17.jpg"  >

Aparecerá la pantalla donde puedes aplicar los filtros, presiona el botón `añadir`. Aparecerán los distintos campos, en los cuales puedes crear el filtrado, selecciona ` CANTIDAD KG `, esto activará un filtro de cantidades numérica en las cuales puedes colocar las diferentes variables.

<img src="../images/08/18.jpg"  >

Luego aplica otro filtro, pero a nivel producto; selecciona el campo `FRUTAS`. Observa que en automático aparecen los distintos tipos de fruta a seleccionar en el catálogo. 
Para este ejercicio, deja sin seleccionar `Palta` y `Plátano`; el filtro dará el total de KG de las frutas seleccionadas.

<img src="../images/08/19.jpg"  >

Si quieres visualizar este dato más detallado y validar que en verdad está tomando solo las frutas que seleccionaste, debes colocar en la parte de filas el campo `frutas` para que desglose el total de las frutas seleccionadas.

<img src="../images/08/20.jpg"  >

Luego aplica, teniendo el filtro a nivel dato, un filtro a nivel vista. Para ello, dirígete a la hoja y posiciónate en los datos de las frutas; observa que al dar clic, habilita un filtrado donde puedes mantener solo ese producto o excluir de la lista el producto.

<img src="../images/08/21.jpg"  >

También puedes mostrar el filtro a la tabla de trabajo, para ello debes arrastrar al campo de filtros el dato de `FRUTAS` y también arrastrar la medida de `TOTALES` que ya se encuentra programada. Sin embargo, debes presionar `control` para pasar la medida a un filtro, como se muestra en las siguientes imágenes. 

<img src="../images/08/22.jpg"  >

También puedes mejorar estos filtros y configurarlos a necesidad del usuario; para ello, posiciona sobre el filtro y da clic sobre la flecha del filtro de `FRUTAS`  como se muestra en las imágenes.

<img src="../images/08/23.jpg"  >


Luego que aprendiste cómo colocar a más detalle los filtros utilizando la información, llegó el momento de armar el primer proyecto; para ello, comienza a combinar información en columnas y filas para que vayas aprendiendo cómo utilizar estos campos con los datos formateados.

Lo primero es colocar en columnas el dato de `FRUTAS` y en filas el campo o dato `NOMBRE DE EMPRESAS`.

<img src="../images/08/24.jpg"  >

#### Actividad sin instrucción guiada
Exporta la base de datos previamente limpiada al programa Tableau Desktop y crea lo siguiente:

- Una tabla de ventas total por CEDIS.
- Una tabla de ventas por VP y Master.
- Una tabla de ventas por artículo por CEDIS.


### Tarea 3. Análisis y filtros en Tableau

Cuando tengas un reporte general, desglosa este reporte. Inicia la representación de los datos en modo de gráfica, para eso necesitas colocar los siguientes datos en filas y columnas.

<img src="../images/08/25.jpg"  >

Del modelo de datos, arrastra de la bd `DATA EXPORTACIÓN` el campo `AÑO ` a la parte de `Páginas`.

<img src="../images/08/26.jpg"  >

El resultado que obtendrás de colocar esta configuración será una gráfica en barras como la siguiente.

<img src="../images/08/27.jpg"  >

Luego, para facilitar la lectura los _storytelling_ utiliza las herramientas para personalizar el gráfico. Para una mejor lectura, coloca las barras de manera vertical utilizando la siguiente herramienta.

<img src="../images/08/28.jpg"  >


El resultado es el siguiente.

<img src="../images/08/29.jpg"  >

Luego, trabaja con la información y pivotea los datos para que ayuden a personalizar la información que necesitas mostrar. Crea, en una nueva hoja de trabajo, una tabla de datos que muestre las ventas por cliente y país. Para ello, arrastra `clientes` a filas.

<img src="../images/08/30.jpg"  >

Donde aparece el _Abc_, coloca en la data `Exportaciones `, las ventas generadas en Canadá.

<img src="../images/08/31.jpg"  >

Luego, aplica lo mismo para los demás países, pero en vez de moverlos donde estaba el _Abc_, colócalos abajo, en la parte de marcas sobre la opción de ` Texto `.

<img src="../images/08/32.jpg"  >

Al mover este dato, su representación no es tan amigable, por lo cual es necesario transformar esta información a tablas de texto; para ello, ve a la opción `mostrar` y selecciona la opción `Tabla de texto`.

<img src="../images/08/33.jpg"  >

El resultado es el siguiente.

<img src="../images/08/34.jpg"  >

Teniendo esta configuración realizada, puedes incluir los demás datos en la parte de nombre `Valores de Medida`, ahí coloca el resto arrastrándolos.

<img src="../images/08/35.jpg"  >

El resultado es el siguiente.

<img src="../images/08/36.jpg"  >

Imagina que son alrededor de 30 países, agregarlos uno por uno sería un trabajo muy estresante y una inefectiva inversión de tiempo.

Para ese tipo de eventualidades y manejo de la información, Tableau tiene una herramienta que se llama pívot, parecido a Excel, pero especializado en el tema de desarrollo o estructuración de datos.

Para utilizar esta herramienta, ve a las fuentes de datos y selecciona la fuente de nombre `DATA EXPORTACIONES`.

<img src="../images/08/37.jpg"  >

Dentro los datos de exportaciones, selecciona las ventas, iniciando en E.E.U.U y finalizando en Canadá; sombrea cada una y da clic derecho para seleccionar la opción pivotar (crear tabla dinámica) en el menú que aparecerá. 

<img src="../images/08/38.jpg"  >


Realizado lo anterior, la data tendrá cambios como se muestra en la siguiente imagen.

<img src="../images/08/39.jpg"  >

Los datos se simplifican y se crean dos campos: el primero con el nombre de las ventas por país y el segundo con el número de ventas.

Si bien, los datos así son funcionales, puedes organizar la data de manera más flexible que pueda ayudar a simplificar y transparentar lo que quieres comunicar en el _storytelling_.

De la nueva columna, solo necesitas extraer los países para crear una estructura más idónea que ayude a organizar la información correctamente.

Para ello, posiciónate sobre esa columna y da clic sobre la pestaña de opciones para que despliegue las herramientas de división.

<img src="../images/08/40.jpg"  >

Realizado lo anterior, observa que crea en automático una columna con los países que tienes en el campo pívot.

<img src="../images/08/41.jpg"  >


Luego, renombra esta columna y la pívot y oculta esa columna.

<img src="../images/08/42.jpg"  >

Realizado el ajuste anterior, la hoja aparecerá toda en rojo, esto es porque que creamos una medida. 

<img src="../images/08/43.jpg"  >

Ya con la medida, puedes realizar la siguiente configuración para el reporte.

<img src="../images/08/44.jpg"  >

La visualización quedará de la siguiente manera.

<img src="../images/08/45.jpg"  >

Para crear una medida en los campos, es necesario posicionarte sobre el modelo de datos y, a continuación, sobre el campo donde deseas agregar la medida.

Para este ejemplo, crea una medida al campo `Cantidad KG` en la cual los kilogramos los convierte a toneladas de la siguiente manera.

Posiciónate sobre los datos de `Data Exportación – campos Cantidad KG`, da clic derecho y selecciona `Crear una medida`.


<img src="../images/08/46.jpg"  >

Ahora que ya sabes crear filtros, crea medidas con la información y juega con las tarjetas que puedes desarrollar para la Dashboard.

Para ello, en esta primera etapa, necesitas colocar el campo de clientes en la parte de columnas y el campo de kilogramos colócalo sobre `Cliente` para obtener la siguiente visualización.


<img src="../images/08/47.jpg"  >

Cuando des clic sobre `Crear campo calculado` aparecerá la siguiente pantalla.

<img src="../images/08/48.jpg"  >

Aquí, coloca las instrucciones para realizar dicha acción, inicia con nombrar este campo como `Cantidad (Tonelada)`.

<img src="../images/08/49.jpg"  >

Ahora, en la parte de las operaciones, coloca lo siguiente: una tonelada es igual a un Kg; por lo tanto, tienes que dividir el campo `Cantidad (KG) ` entre mil.

<img src="../images/08/50.jpg"  >

Acéptalo y aparecerá este nuevo campo en el modelo. Mueve el campo hacia texto y mira qué sucede.

<img src="../images/08/51.jpg"  >

Mostrará la tarjeta aparte de los Kg, también aparecerán las toneladas.

<img src="../images/08/52.jpg"  >

Ahora imagínate que te piden redondear este valor de tonelada, para ello vamos al campo que creamos de cantidad tonelada y editamos la medida, para redondear agregaremos a la formula la instrucción ROUND y en ella especificamos la cantidad de decimales de la siguiente manera:

<img src="../images/08/53.jpg"  >

Si observamos bien este redondeo que aplicamos no nos ayudó mucho en el tema de los valores:

<img src="../images/08/54.jpg"  >

Analicemos la raíz de nuestra información porque a nivel aplicativo no creo que sea el error, esto viene desde la raíz, vamos al Excel de Data Exportaciones para entender los datos

<img src="../images/08/55.jpg"  >

Lo primero será activar filtros y filtrar la primera empresa para ellos debemos de validar que numero de empresa es America Exportadores y filtramos el Id cliente número 3

<img src="../images/08/56.jpg"  >


Ahora seleccionemos todos los datos de nuestra columna D de nombre Cantidad (KG).

<img src="../images/08/57.jpg"  >

Observemos que el promedio de datos nada que ver con los datos que tenemos en nuestro informe. ¿Equipo la pregunta del millón porque está pasando esto ?, ¿Acaso los datos los introducimos o exportamos mal ?

Ahora vamos con la REPUESTA, recuerdan que creamos una pívot y 5 filas las unimos a una sola, entonces si esa cantidad que nos da Excel la multiplicamos por 5 nos dará la misma cantidad.

<img src="../images/08/58.jpg"  >


La explicación lógica resuelta pero como presentamos esta información, tenemos que realizar unos ajustes en nuestra formula de la medida, donde colocaremos la suma de las cantidades de KG divididas entre 1000 y ahí aplicaremos nuestra instrucción de ROUND y quedara de la siguiente manera equipo:

<img src="../images/08/59.jpg"  >

El resultado es :

<img src="../images/08/60.jpg"  >


### Tarea 4. Dashboards e Historias

Si miramos bien, nuestra primera tarjeta nos presenta dos datos, las cantidades en kilogramos y las cantidades en toneladas, pero a nosotros nos interesa solo quedarnos con toneladas por lo tanto en esta primera tarjeta vamos a quitar la cantidad en kilogramos.

<img src="../images/08/61.jpg"  >

Ya tenemos la representación de los datos que necesitamos, ahora vamos a personalizar nuestra tarjeta y para ellos el primer dato que vamos a modificar es el título de la tarjeta, el cual dice Clientes, no nos interesa ese título por lo tanto lo vamos a eliminar de la siguiente manera.

Daremos clic derecho sobre el titulo y presionaremos donde dice ocultar:

<img src="../images/08/62.jpg"  >

Quedando como resultado la siguiente imagen:

<img src="../images/08/63.jpg"  >

Ahora vamos a cambiar el nombre de la hoja presionando sobre hoja dos y colocaremos el nombre de TONELADAS POR CLIENTE:

<img src="../images/08/64.jpg"  >

Observemos que al momento de hacer el cambio el título de nuestra paleta de trabajo también cambio de hoja 2 a Toneladas por Cliente, también vamos a personalizar ese título y colocaremos Descripción – Toneladas Clientes, lo haremos de la siguiente manera:

<img src="../images/08/65.jpg"  >

Personalizado el título daremos clic en aceptar y el resultado será el siguiente:

<img src="../images/08/66.jpg"  >

Ahora nos toca formatear los valores de  nuestra tarjeta para ello daremos clic derecho sobre el primer valor y nos aparecerá las siguientes opciones:

<img src="../images/08/67.jpg"  >

Lo primero que vamos a realizar con esta herramienta de formateo es personalizar los títulos de cliente, para ellos observemos en la siguiente imagen que podemos seleccionar que dato es el que queremos formatear:

<img src="../images/08/68.jpg"  >

Ahora que seleccionamos el campo cliente , haremos las siguientes modificaciones en nuestro panel de personalización: 

<img src="../images/08/69.jpg"  >

El resultado será el siguiente:

<img src="../images/08/70.jpg"  >

A continuación, vamos a centrar el texto del campo clientes, daremos clic en la opción de Alineación y seleccionaremos la alineación central:

<img src="../images/08/71.jpg"  >

El resultado es :

<img src="../images/08/72.jpg"  >

Nuestro texto de cliente ya está alineado y formateado, ahora toca selecciona las cantidades en toneladas, para ello seleccionamos el campo primero:

<img src="../images/08/73.jpg"  >

Procedemos a colocar el siguiente formateo: 

<img src="../images/08/74.jpg"  >

Para alinear seleccionaremos la opción alineación de la siguiente manera:

<img src="../images/08/75.jpg"  >

Seleccionamos alineación y justo en esa opción, nos vamos a la sección de Predeterminado y en panel colocamos alineación central como se muestra en la imagen:

<img src="../images/08/76.jpg"  >

Obtendremos el siguiente resultado:

<img src="../images/08/77.jpg"  >

Ahora vamos a quitar las líneas divisoras de nuestros datos para realizar este ajuste vamos a dar clic cobre la opción Limites y buscaremos la opción Divisor de Filas aquí quitamos estas líneas como lo muestro en las siguientes imágenes: 

<img src="../images/08/78.jpg"  >

El resultado es el siguiente sin estas líneas divisoras, cabe recalcar que ustedes pueden colocar el formateo que más les agrade:

<img src="../images/08/79.jpg"  >

Ahora vamos a formatear el valor, como vemos nos aparece un decimal en 0, ese decimal vamos a quitarlo de la siguiente manera, vamos a seleccionar en la parte de campos cantidad en toneladas, ya que esta seleccionada nos vamos a ir a la pestaña de panel ahí buscaremos la opción de números daremos clic y seleccionaremos la opción Números Estándar.

<img src="../images/08/80.jpg"  >

Realizado ese formateo, el resultado es el siguiente:

<img src="../images/08/81.jpg"  >

Ahora parte de la personalización es también la organización de nuestros datos, si analizamos bien hay bastantes datos o campos que no son necesarios para nuestro dashboard por lo tanto vamos a ocultarlos desde nuestra fuente de datos de la siguiente manera:

Primero vamos a nuestra pestaña de fuente de datos:

<img src="../images/08/82.jpg"  >

Ya dentro de nuestra pestaña de datos primero trabajaremos con nuestra conexión de nombre Data Exportaciones, aquí quitaremos todos los ID, vamos a proceder ocultarlo para ello seleccionaremos el primero que es Id Empresas daremos clic sobre su pestaña de opciones y seleccionaremos ocultar como se muestra en la imagen, realizado esto procederemos hacer lo mismo para los demás ID

<img src="../images/08/83.png"  >

El resultado que debemos tener es el siguiente:

<img src="../images/08/84.jpg"  >

Ahora procedemos a realizar lo mismo ocultar todos los ID de las demás conexiones (Clientes, Empresas, Frutas)

El resultado esperado es el siguiente:

<img src="../images/08/85.jpg"  >

Si nosotros necesitamos mirar los valores ocultos, podemos visualizarlo donde clic sobre el engrane como se muestra en la siguiente imagen y con esto les aparecerán habilitado y sombreados estos campos ocultos

<img src="../images/08/86.jpg"  >


Ahora la pregunta del millón, ¿ esto para que me sirve? Miremos un antes y un después en nuestra tabla de trabajo a nivel campos:

<img src="../images/08/87.jpg"  >

Esta organización de nuestra información nos ayudara de una manera más fácil identificar los campos y los valores a utilizar en nuestro Dashboard.
Realizado lo anterior procederemos a crear un diagrama de barra personalizado, para ello iniciaremos creando una nueva hoja en nuestra tabla de trabajo.

<img src="../images/08/88.jpg"  >

Creada la hoja le colocaremos el nombre de Toneladas de frutas por Cliente.

<img src="../images/08/89.jpg"  >

Personalizada nuestra nueva hoja, lo primero que realizaremos es arrastra nuestro campo de clientes a columna y en la parte de valores colocaremos el campo calculado que creamos anteriormente de nombre Cantidad (Toneladas).

<img src="../images/08/90.jpg"  >

Colocado los campos , ahora nos iremos a nuestro menú MOSTRAR y seleccionaremos Barras Horizontales y rotamos este grafico con la opción de rotación 

<img src="../images/08/91.jpg"  >

De esta forma en el eje Y tenemos las Toneladas en el eje X tenemos los distintos clientes, ahora nosotros también necesitamos saber la exportación que se ha tenido de las diferentes frutas para ellos arrastraremos el campo de frutas a la parte de columnas y presionaremos en la herramienta de mostrar etiquetas.

<img src="../images/08/92.jpg"  >

Ahora ayúdenme a que su desarrollo quede como les comparto en la siguiente imagen.

<img src="../images/08/93.jpg"  >

Ya formateado nuestro grafico como les mostraba anteriormente es necesario colocar en las columnas colores por clientes, esto para que nos ayude a visualizar de mejor manera los datos , procederemos a realizar lo siguiente primero arrastraremos nuestro campo de clientes a la herramienta de colores. Que sucederá al aplicar este tipo de filtrado, colocará a cada cliente un color distinto como lo Muestro en la siguiente imagen.

<img src="../images/08/94.jpg"  >

También nosotros podemos formatear que nuestro grafico de barras lo coloque de manera descendente y la tarjeta de colores la podemos ocultar esto para dar una mejor vista a nuestro reporte.

<img src="../images/08/95.jpg"  >

Ahora ocultaremos el encabezado de la gráfica dando clic derecho ocultar.

<img src="../images/08/96.jpg"  >

Por último, vamos a formatear para que no esté apareciendo el decimal que muestra nuestra grafica en el total de toneladas, para ellos iremos a la medida y daremos clic izquierdo y presionamos en formatear en la pestaña de Panel nos iremos a la opción de números y colocaremos Numeración Estándar.

<img src="../images/08/97.jpg"  >

El resultado es el siguiente:

<img src="../images/08/98.jpg"  >

Ahora crearemos otra hoja la cual le colocaremos el nombre de Monto total y porcentaje por país.

<img src="../images/08/99.jpg"  >

Ahora vamos a necesitar el campo de País en Filas y necesitamos el monto total de la venta para ellos analicemos nuestro Excel de Data Exportaciones.

<img src="../images/08/100.jpg"  >

Para obtener ese total de monto será necesario crear una medida en la cual multipliquemos cantidad kg por la venta de los países. 

Lo primero que debemos ubicar el campo de precio y daremos clic derecho y crearemos un campo calculado.

<img src="../images/08/101.jpg"  >


Creado el campo monto total ahora si vamos a iniciar a desarrollar nuestra grafica por lo cual colocaremos en filas el campo Países y como valores colocaremos el campo que acabamos de crear Monto Total.

<img src="../images/08/102.jpg"  >

Ahora con esta pequeña tabla ya colocada vamos a el menú Mostrarme y colocaremos una gráfica en barra y miren lo que sucede:

<img src="../images/08/103.jpg"  >

Ahora que pasara si de nuevo colocamos en columnas nuestro campo calculado de monto total.

<img src="../images/08/104.png"  >

Si observamos bien nos aparece el mismo dato en diferentes graficas de barras colocadas, pero esta segunda grafica nos ayudara a calcular el porcentaje por lo cual daremos clic derecho sobre el segundo campo calculado de monto total y seleccionaremos, Calculo de tablas rápido la opción de Porcentaje del Total y miremos que sucede

<img src="../images/08/105.jpg"  >

Vamos a irnos a nuestro segundo campo agregado de monto total y daremos clic sobre él , seleccionaremos en el menú la opción que dice discreto y observemos.
<img src="../images/08/106.jpg"  >

Ahora solo es cuestión de formatear la información del porcentaje y dejarlo solo con 2 cifras para ellos vamos a Suma Monto Total de filas y damos clic, después formatear y colocaremos lo siguiente:

<img src="../images/08/107.jpg"  >

Ahora solo coloquemos nuestro grafico de forma Descendente y el resultado es :

<img src="../images/08/108.jpg"  >

Ahora vamos a personalizar los colores de nuestro grafico para ellos vamos a arrastrar el campo de monto total a la parte de colores y miremos cómo se comporta:

<img src="../images/08/109.jpg"  >

Vamos a personalizar ese azul y lo cambiaremos por otro color desde la paleta que se creó a la derecha de nuestro desarrollo, miremos el resultado.

<img src="../images/08/110.jpg"  >

Ya que creamos nuestra grafica de barras de total y porcentaje ahora vamos a crear una nueva hoja de trabajo donde le colocaremos por título Filtro de Donas.

<img src="../images/08/111.jpg"  >

La primera acción para realizar es que vamos a arrastrar el dato de País a la herramienta colores:

<img src="../images/08/112.jpg"  >

Como resultado nos aparece nuestro dato de la siguiente manera:

<img src="../images/08/113.jpg"  >

Ahora en la parte de marcas vamos a dar clic en la lista desplegable y seleccionaremos Circular.

<img src="../images/08/114.jpg"  >


Al realizar la acción pasada el resultado que nos mostrara es el siguiente:

<img src="../images/08/115.jpg"  >

A continuación, vamos a iniciar a armar nuestro gráfico y como segundo dato vamos arrastra Cantidad (Toneladas) a etiquetas:

<img src="../images/08/116.jpg"  >

Ahora vamos a crear nuestro Placeholder de la siguiente manera en la parte de columnas daremos doble clic y colocaremos un 1 y de nuevo daremos doble clic y colocaremos 2, esta acción formateara nuestra grafico de la siguiente manera:

<img src="../images/08/117.jpg"  >

Ahora En el valor 1 daremos clic izquierdo y en el menú crearemos esta acción en una dimensión lo mismo para el valor 2.

<img src="../images/08/118.jpg"  >

El resultado al dar clic sobre dimensión en ambos valores de las columnas , nuestra grafica de pastel quedara de la siguiente manera:

<img src="../images/08/119.jpg"  >

Ahora personalizaremos la vista, para ellos daremos clic la opción de vista y cambiaremos de Estándar a Vista Completa:

<img src="../images/08/120.jpg"  >

Esto nos ayudara a crecer nuestra área de trabajo y daremos una mejor visualización y presentación de nuestra gráfica:

<img src="../images/08/121.jpg"  >

Al crear este tipo de formateo, Observemos que la parte de marcas se nos agregaron la configuración de nuestras graficas de pastel de manera independiente:

<img src="../images/08/122.jpg"  >

Vamos a iniciar la personalización e iniciaremos con el grafico Uno, en este vamos a crecer la gráfica al segundo espacio, iniciaremos dando clic en tamaño como muestro en la imagen:

<img src="../images/08/123.jpg"  >

Ahora vamos a realizar algunos ajustes en el grafico Dos, daremos clic sobre él y quitaremos el dato de País y nos quedara un círculo en gris y con el Total de Toneladas.

<img src="../images/08/124.jpg"  >

Ahora daremos clic izquierdo sobre el valor dos en columnas y seleccionaremos Eje Doble:

<img src="../images/08/125.jpg"  >

Seguiremos personalizando el valor Dos , vamos a seleccionar dentro  de marcas sobre el valor dos un color y seleccionaremos el color blanco para obtener este resultado:

<img src="../images/08/126.png"  >

Ahora personalicemos nuestro Dato Uno (Grafico Uno) vamos a agregar las etiquetas de país en sus valores de la siguiente manera:

<img src="../images/08/127.jpg"  >

Nosotros podemos también formatear que en vez de aparecer el número de toneladas nos represente el dato el porcentaje del total de toneladas por país y esto lo realizaremos de la siguiente manera, daremos clic izquierdo en Cantidad (Toneladas) , luego daremos en calculo tablas rápido y seleccionamos la opción Porcentaje de Total nos mostrara la información de la siguiente manera:

<img src="../images/08/128.jpg"  >

Coloquemos más datos informativos en esta gráfica, arrastremos de nuevo Cantidad (Toneladas) a etiquetas y observemos la representación de nuestros valores a nivel porcentaje y numéricamente el valor de las toneladas.

<img src="../images/08/129.jpg"  >

Ahora vamos a quitar los encabezados de nuestra tabla de trabajo que nos aparecen arriba y abajo (1,2), para ellos daremos clic derecho en el encabezado 1 y seleccionaremos la opción Mostrar encabezado esto para que desactive estos títulos:

<img src="../images/08/130.jpg"  >

Ahora quitaremos esa línea divisora, para ellos daremos clic izquierdo opción formatear y seleccionaremos la opción línea, dentro de esta opción colocaremos como Ninguna  , Líneas Cuadricula y Línea Cero.

<img src="../images/08/131.jpg"  >

Creadas estas gráficas y nuestras tablas estamos listos para crear nuestro primer Dashboard para estos datos, para ellos vamos a dar clic en crear un dashboar en la siguiente opción:

<img src="../images/08/132.jpg"  >

Creado nuestra Dashboard lo primero que tenemos que realizar es configurar la pantalla de visualización lo recomendable es coloca una visualización automática, esto para que se ajuste al monitor de cada usuario.

<img src="../images/08/133.png"  >

Ahora configurada nuestra visualización lo primero que arrastraremos será nuestra tabla de Toneladas por Cliente y daremos clic sobre su fecha de herramientas y configuraremos su visualización a vista completa de la siguiente manera:

<img src="../images/08/134.jpg"  >

Ahora arrastremos nuestra grafica de barras de Toneladas de Frutas por cliente y está la colocaremos en la parte inferior como se muestra en la siguiente imagen:

<img src="../images/08/135.jpg"  >


Ahora arrastraremos nuestra grafica de nombre Monto total y porcentaje país y este lo colocaremos también en la parte inferior, solo que al momento de soltarlo será necesario que demos un ajuste para poder representar bien nuestros datos que componen este Dashboard.

<img src="../images/08/136.jpg"  >

Ya tenemos nuestros 3 componentes de nuestro Dashboard pero es necesario quitar los títulos de los 2 últimos componentes para ellos vamos a dar clic sobre la pestaña de opciones y desactivaremos los títulos como se muestra en la imagen:

<img src="../images/08/137.jpg"  >

Ahora agregaremos nuestro filtro de donas este lo arrastraremos a la derecha de nuestro componente Monto total y porcentaje como se muestra en la imagen, recordemos quitar el título :

<img src="../images/08/138.jpg"  >

Para dar una mejor apariencia a nuestro dashboard es necesario validar que el encuadre de nuestros componentes sea Vista Completa como se muestra en la imagen: 

<img src="../images/08/139.jpg"  >

Validado lo anterior ahora nos tocará agregar algunos filtros importantes para esta implementación,  primer filtro será de clientes y este lo generaremos de nuestra tabla de Toneladas Clientes directo en las opciones desplegables como se muestra en la siguiente imagen:

<img src="../images/08/140.jpg"  >

Ahora agregaremos un filtro que contenga las frutas y este filtro lo generaremos desde nuestro componente Tonelada de frutas por cliente como lo realizamos anterior mente solo que ahora en automático lo colocara debajo de clientes:

<img src="../images/08/141.jpg"  >

Al aplicar el filtro el resultado es el siguiente:

<img src="../images/08/142.jpg"  >

Si miramos bien esta manera de colocar los filtros no es tan conveniente, por lo tanto, editaremos el filtro de clientes y lo personalizaremos desde su pestaña de ajustes: 

<img src="../images/08/143.jpg"  >
