# Proyecto Final

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
1.	xxxxxx


## Objetivo Visual 

<img src="../images/01/00.png" width="500" >



## Duración aproximada:
- 120 minutos.


## Instrucciones 

### Tarea 1. Analisis de datos

1. Para este primer ejercicio es necesario descargar el material de la carpeta de nombre Primer Proyecto / Data, mismo que ya tiene en su alcance con el material que se les proporciono. 

2. Lo primero que vamos a realizar es analizar la data que se nos está proporcionando y realizar nuestra primera inspección de limpieza de datos:

<img src="../images/08/01.png" width="400" >
<img src="../images/08/02.png" width="400" >
<img src="../images/08/03.png" width="400" >

### Tarea 2. Desarrollar un dashboard

*Objetivo:* Desarrollar una Dashboard que nos permita analizar la cantidad de Toneladas de fruta que se han exportado a los clientes de distintos países.

¿ Que se requiere ? 
- Cantidad de Toneladas por Cliente.
- Cantidad de Toneladas por Empresa.
- Cantidad de Tonelada de Clientes por Fruta.
- Ganancias de Exportación por País.
- % de las Ganancias de los Países del Monto Total.
- % de las Exportaciones en Toneladas por País.

<img src="../images/08/04.png" width="400" >


Ya que conocemos el objetivo y los puntos que nos están solicitado, es momento de organizar la data por lo cual te pido crear una carpeta dentro de equipo de cómputo donde organicemos de la siguiente manera los archivos:
<img src="../images/08/05.png" width="400" >

Lo primero es organizar nuestro archivo para posterior mente a esto ahora si vamos a crear nuestra conexión de nuestra data a nuestra aplicación Tableau.

Lo primero que tenemos que hacer es conectar los distintos archivos de data que tenemos en nuestro desarrollo para ellos vamos a abrir nuestra aplicación de Tableau Desktop e iremos a la primera pantalla junto donde aparecen el letrero CONECTAR

<img src="../images/08/06.jpg" width="400" >

Vamos a conectar primero nuestra data generada en Excel (Data Exportaciones), presionamos abrir 

<img src="../images/08/07.jpg" width="400" >

al dar clic en abrir nos colocara nuestra data ya en nuestra paleta de datos , ahora vamos a exportar esta información a nuestro aplicativo, arrastrando primero DATA EXPORTACIONES y posteriormente CLIENTES.
OJO Observemos que cuando arrastramos ambas hojas (data) en automático el aplicativo crea una conexión, crear una relación entre ambas tablas.

<img src="../images/08/08.jpg" width="400" >


Ahora nos toca crear la conexión con nuestro archivo TXT. de nombre FRUTAS, para ello procederemos a realizar lo siguiente:  

<img src="../images/08/09.jpg" width="400" >

Ya que seleccionamos el tipo de data como texto, seleccionaremos nuestro texto formateado de FRUTAS dando clic en abrir.

<img src="../images/08/10.jpg" width="400" >


Realicemos el mismo proceso que realizamos con nuestra data de Excel, arrastremos a nuestra paleta de trabajo y observemos que en automático de nuevo crea esta relación de información.
<img src="../images/08/11.jpg" width="400" >

Llego el momento de unir nuestra última data el CSV de nombre Empresas a nuestro proyecto en Tableau. 
<img src="../images/08/12.jpg" width="400" >


Ya que dimos clic sobre data CSV , seleccionamos la carpeta empresas y damos clic sobre el archivo Empresas.
<img src="../images/08/13.jpg" width="400" >

Llego el momento crear esta conexión de datos, vamos a arrastrar nuestro archivo y observemos que sucede, este archivo debemos de enlazarlo directo a nuestro archivo principal.
<img src="../images/08/14.jpg" width="400" >

Si observamos bien nos presenta un error al realizar nuestra relación , no identifica que campos unir, aquí la importancia de conocer nuestra data con la que vamos a trabajar para brinda una estructura correcta en esta primera fase y muy importante porque es nuestro cimiento de nuestro Dashboard.

¿ Como solucionarlo ?, es sencillo equipo vamos a unir nuestra data de ambos archivos con el campo Id Empresas.

<img src="../images/08/15.jpg" width="400" >

Ahora que ya tenemos nuestras conexiones en nuestras diferentes conexiones de datos, llego el momento de realizar nuestra visualización de datos, lo primero es que vamos a aplicar un filtro a nivel Origen.

Vamos a irnos a la pestaña de Hoja1 y vamos a seleccionar de nuestros datos DATA EXPORTACION seleccionaremos el cambo CANTIDAD EN KG

<img src="../images/08/16.jpg" width="400" >

Ya que estamos en nuestra pestaña de fuente de datos, vamos a dar clic en añadir filtros.
<img src="../images/08/17.jpg" width="400" >

Nos aparecerá la pantalla donde podemos aplicar los filtros, presionaremos en el botón añadir, nos aparecerán los distintos campos en los cuales podemos crear el filtrado, seleccionaremos CANTIDAD KG, esto nos activara un filtro de cantidades numérica en las cuales podemos coocar las diferentes variables.

<img src="../images/08/18.jpg" width="400" >

Ahora apliquemos otro filtro, pero a nivel producto, seleccionaremos el campo FRUTAS, observemos que en automático nos aparece los distintos tipos de fruta a seleccionar de nuestro catálogo, para este ejercicio dejare sin seleccionar Palta y Plátano , lo que el filtro hará es solo darme el total de KG de esas frutas que seleccionamos.
<img src="../images/08/19.jpg" width="400" >


Justo si queremos visualizar este dato más a detallado y validar que en verdad está tomando solo las frutas que seleccionamos, deberemos de colocar en la parte de filas el campo frutas para que nos desglose ese total entre las frutas seleccionadas.
<img src="../images/08/20.jpg" width="400" >

Ahora aplicaremos teniendo nuestro filtro a nivel dato, un filtro a nivel vista, para ellos vamos a nuestra hoja 1 y nos posicionamos en nuestros datos de las frutas, observemos que al dar clic sobre nos habilita un filtrado donde podemos mantener solo ese producto o excluir de la lista ese producto.

<img src="../images/08/21.jpg" width="400" >

También podemos mostrar nosotros nuestro filtro a nuestra tabla de trabajo, para ellos debemos de arrastrar al campo de filtros el dato de FRUTAS y podríamos también arrastrar la medida de TOTALES que ya se encuentra programada, pero ojo debemos presionar control para pasar nuestra medida a un filtro, como se muestra en las siguientes imágenes.

<img src="../images/08/22.jpg" width="400" >

Estos filtros también podemos mejorarlos y configurarlos a necesidad del usuario, para ello nos posicionamos sobre el filtro y daremos clic sobre la flechita del filtro de frutas como se muestra en las imágenes.

<img src="../images/08/23.jpg" width="400" >


Ahora que aprendimos como colocar a más detalle nuestros filtros utilizando nuestra información llego el momento de ir armando nuestro primer proyecto , para ellos vamos a iniciar a combinar información en columnas y filas para que vallamos aprendiendo como utilizar estos campos con nuestros datos formateados.

Lo primero es que vamos a colocar en columnas nuestro dato de FRUTAS y en filas el campo o dato NOMBRE DE EMPRESAS.

<img src="../images/08/24.jpg" width="400" >

Instrucción: En base a la base de datos que limpiamos anteriormente vamos a exportarla a nuestro programa de Tableau Desktop y vamos a crear lo siguiente Tabla de ventas total  por Cedis , Tabla de venta por VP Y Master y por último una Tabla de ventas por Articulo por Cedis



