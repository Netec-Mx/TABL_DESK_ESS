# Conexión y preparación de datos

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
1. Conectarse a una fuente de datos en Tableau Desktop (por ejemplo archivo, servidor o servicio en la nube) y abrir la sesión inicial.
2. Visualizar la página de “Conectar” en Tableau, elegir un conector y vincular el conjunto de datos “Muestra - Supertienda”. 
3. Ver la interfaz de fuente de datos: observar la hoja de trabajo en blanco, la lista de campos, los tipos de dato y roles que asigna automáticamente Tableau. 

https://help.tableau.com/current/guides/get-started-tutorial/es-es/get-started-tutorial-connect.htm 
## Objetivo Visual 

<img src="../images/01/00.png" width="500" >

## Duración aproximada:
- 20 minutos.

## Instrucciones 

Su jefa le pidió que mirara las ventas y la rentabilidad general de la empresa para detectar las principales áreas de mejora. Tiene un montón de datos, pero no sabe por dónde empezar. Decide empezar con una versión de prueba gratuita de Tableau Desktop.

### Tarea 1. 

Lo primero que ve después de abrir Tableau Desktop es la página de inicio. Aquí puede seleccionar el conector (el modo en que se conectará a los datos) que quiera utilizar.

<img src="../images/01/01.png" width="500" >

La página de inicio ofrece varias opciones entre las que elegir:

1.	Icono de Tableau. Haga clic en <img src="../images/01/02.png" > situado en la esquina superior izquierda de cualquier página, para cambiar de la página de inicio al área de trabajo de creación y viceversa.

2.	Conectar panel. En Conectar, puede:

- Conectarse a datos almacenados en un archivo, como Microsoft Excel, PDF y archivos espaciales, entre otros.
- Conectarse a datos almacenados en Tableau Server, Microsoft SQL Server, Google Analytics, u otro servidor.
- Conectarse a una fuente de datos a la que se haya conectado antes.

Tableau admite la posibilidad de conectarse a una amplia variedad de datos almacenados en una gran cantidad de sitios. En el panel Conectar aparecen las ubicaciones más habituales a las que puede conectarse. También puede hacer clic en los vínculos Más para ver más opciones. Para obtener más información sobre cómo conectarse a fuentes de datos, consulte la Biblioteca de aprendizaje para este tutorial.

3. En Aceleradores, vea una selección de Aceleradores y los libros de trabajo de muestra que se incluyen con Tableau Desktop. Antes de 2023.2, estos se llamaban libros de trabajo de muestra.

4. En Abrir, puede abrir libros de trabajo que ya ha creado.

5. En Descubrir, encontrará recursos adicionales como tutoriales de vídeo, foros o la sección "Viz of the week" para obtener ideas sobre lo que puede crear.

En el panel Conectar, en Fuentes de datos guardadas, haga clic en Muestra - Supertienda para conectarse al conjunto de datos de ejemplo.

<img src="../images/01/03.png" width="500" >

Después de seleccionar Muestra - Supertienda, su pantalla tendrá este aspecto:

<img src="../images/01/04.png" width="500" >

El conjunto de datos Muestra - Supertienda se suministra con Tableau. Contiene información sobre productos, ventas, ganancias, etc. que puede utilizar para identificar áreas clave para su mejora dentro de esta compañía ficticia.

###¿Qué hace Tableau con los datos?

Después de conectarse a los datos, Tableau procede del modo siguiente:

- Abre una nueva hoja de trabajo. Se trata de un área en blanco en la que puede crear su primera vista.
- Muestra la fuente de datos a la que se ha conectado. Si utiliza varias fuentes de datos, las verá todas aquí.
- Agrega columnas de la fuente de datos al panel Datos de la izquierda. Las columnas se agregan como campos.
- Asigna automáticamente tipos de datos (como la fecha, el número, la cadena, etc.) y roles (dimensión o medida) a sus datos. (Hablaremos más sobre estos términos más adelante).

Si desea conocer todos los detalles sobre los datos, puede seleccionar la página Fuente de datos en la esquina inferior izquierda. Aquí puede ver las primeras 1000 filas de datos y esto enloquece a algunos analistas: ordenar u ocultar campos, dividir campos en varias columnas y cambiar el nombre de los encabezados de columnas, todo sin modificar los datos originales. Lo que pasa en Tableau se queda en Tableau: sus datos están protegidos.

Si ha ido a la página Fuente de datos para consultar los detalles, haga clic en la pestaña de Hoja 1 para volver al punto de inicio.
