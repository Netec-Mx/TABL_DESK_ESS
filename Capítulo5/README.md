# Práctica 5. Análisis avanzado

## Objetivos
Al finalizar la práctica, serás capaz de:
- Diseñar visualizaciones avanzadas.
- Crear un dashboard con gráficas y análisis avanzados.


## Objetivo visual 

<img src="../images/05/00.png" width="500" >



## Duración aproximada
- 120 minutos.


## Instrucciones 

### Tarea 1. Análisis avanzados

Para este desarrollo es necesario descargar la data que tenemos en nuestra carpeta de nombre Segundo Proyecto:

Por favor para continuar con el desarrollo del proyecto se tiene que crear una carpeta y descargar el archivo "Data.zip", una vez descargado tienes que extraer los archivos que contienen. Tales archivos contienen los siguientes nombres:

*Crear Carpeta -> "Dashboard - Recursos Humanos"*
*Data.xlsx*
*ESQUEMA_RRHH.jpg*
*Background.jpg*


Ya que tenemos nuestra data en nuestro escritorio vamos a analizar nuestro archivo tomando como base este diagrama: 

<img src="../images/05/01.jpg"  >


Explicada el desarrollo de nuestra dará y el relacionamiento que tenemos que colocar en el procederemos a iniciar a desarrollar nuestro proyecto.

Para ello cargaremos nuestro archivo de Excel de nombre DATA seleccionando el tipo de formato de archivo que utilizaremos.

<img src="../images/05/02.jpg"  >

Ya cargado nuestra data nos aparecerá de la siguiente manera:

<img src="../images/05/03.jpg"  >

Lo primero que colocaremos será nuestra tabla de Empleados (Employee) y arrastraremos también nuestra Tabla de trabajo (job) estas se relacionaran ambas con el campo JOB ID

<img src="../images/05/04.jpg"  >

Ahora arrastraremos el campo Historial de trabajos (job_History) y este lo relacionaremos con nuestra tabla de Trabajos (job) ambos por el campo JOB ID.

<img src="../images/05/05.jpg"  >

Ahora arrastraremos la tabla Departamento (Department) y está la relacionaremos con nuestra tabla de Empleados (Employee) ambos por el campo Departmen ID.

<img src="../images/05/06.jpg"  >


Ahora arrastraremos la tabla Ubicaciones (Locations) y este lo relacionaremos con nuestra tabla de Departamento (Department) ambos por el campo Location ID.

<img src="../images/05/07.jpg"  >

Ahora arrastraremos la tabla Estado (Countries) y está la relacionaremos con nuestra tabla de Ubicaciones (Locations) ambos por el campo Country ID.

<img src="../images/05/08.jpg"  >

Finalmente  arrastraremos la tabla Region y este lo relacionaremos con nuestra tabla de Estado (Countries) ambos por el campo Region ID.

<img src="../images/05/09.jpg"  >

El resultado final de nuestra data es el siguiente : 

<img src="../images/05/10.jpg"  >

Ahora equipo para darle una mejor estructura a nuestro modelo de datos vamos a ir tabla por tabla y ocultaremos los campos que no será necesarios para nuestro manejo de datos, estos campos solo nos ayudarían a relacionar y crear nuestro modelo.

Estos campos serán todos los ID de nuestras tablas como se muestra en la imagen:

<img src="../images/05/11.jpg"  >

Ya que ocultamos estos campos que no son necesarios para nuestro desarrollo, daremos clic sobre hoja 1 y nos aparecerán nuestros datos de la siguiente manera:

<img src="../images/05/12.jpg"  >

Vamos a probar que esta  todo bien, para ellos en filas colocaremos el campo First Name y como dato colocaremos el campo  Salary para que nos presente el siguiente listado:

<img src="../images/05/13.jpg"  >

Ahora crearemos un campo calculado donde unamos nuestro campo First Name más el campo Last Name de la siguiente manera

<img src="../images/05/14.jpg"  >

Ya que validamos que todo está en orden vamos a remover los datos anteriores de nuestra tabla de trabajo y ahora arrastraremos el campo Hire Date ( Fecha de Contratacion) y Nombre en columnas  y en filas colocaremos el campo Salary.
Realizado esto vamos a presionar en formatear sobre nombre y colocaremos nuestros nombres centrados de manera Horizontal como se muestra en la siguiente imagen.

<img src="../images/05/15.jpg"  >

Creado nuestro grafico de salarios, vamos a irnos a nuestra pestaña de Análisis, conozcamos más de esta herramienta.

| Herramienta  | Función |
| ------------- | ------------- |
| Pestaña de Análisis  | herramienta para explorar patrones, tendencias y detalles en datos. |
| Arrastrar y soltar objetos analíticos | líneas, bandas, áreas, totales → destacan aspectos clave.  |
| Líneas de referencia  | promedios, medianas, mínimos o máximos → contextualizan datos  |
| Barras de referencia  | marcan rangos o límites específicos en la visualización |
| Líneas de tendencia  | muestran comportamiento en el tiempo o frente a otra variable (lineal, exponencial, logarítmico) |
| Previsiones | proyectan tendencias futuras con base en datos históricos |
| Cálculos rápidos de tabla  | porcentajes, diferencias, totales → aplicados desde pestaña Análisis.  |
| Resaltado | reglas para identificar valores atípicos o áreas de interés  |
| Agrupación y clústeres  | grupos automáticos según similitudes en los datos  |

Soltamos y observemos que nos solicita un valor para este ejemplo colocaremos $12,000  que será nuestra línea constante, esta nos sirve para analizar los datos que sobre pasen este tope de valor, es por ellos que a lo largo del grafico coloca una línea Horizontal con un valor de 12,000.

<img src="../images/05/16.jpg"  >

Esta constante también la podemos formatear si fuera nuestra necesidad desde cambiar el valor hasta personalizar la línea dando clic sobre él nos aparecerá un menú donde podemos acceder a estos ajustes como muestro en la siguiente imagen:

<img src="../images/05/17.jpg"  >

Vamos a dar clic sobre la opción Formatear en esta opción nosotros podemos personalizar nuestra línea desde la forma, color y grosor, como se muestra en la siguiente imagen: 

<img src="../images/05/18.jpg"  >

Ahora iremos de nuevo a nuestra pestaña de análisis y arrastraremos la opción de Línea de Promedio nos aparecerá una su opción donde especificaremos la línea de referencia que tomará como se muestra en la siguiente imagen donde seleccionaremos como tabla: 

<img src="../images/05/19.jpg"  >

Si observamos nos aparece una línea igual que constante solo que aquí nos señala el promedio de salarios que estamos teniendo.

<img src="../images/05/20.jpg"  >

Ahora eliminaremos la línea de nuevo iremos a nuestra pestaña de análisis y seleccionaremos línea promedio solo que ahora seleccionaremos la opción de Panel como se muestra en la imagen:

<img src="../images/05/21.jpg"  >

Ahora si observamos esta opción nos muestra los promedios por panel por cada sección como se muestra en la imagen:

<img src="../images/05/22.jpg"  >

Ahora de nuevo eliminamos la línea y vamos por nuestra última opción en línea de referencia, pero ahora por celda:

<img src="../images/05/23.jpg"  >

Justo en esta opción nos ayudara a ver el promedio por cada una de las celdas o columnas para poder realizar una visión de crecimiento más adecuada como se muestra en la imagen:

<img src="../images/05/24.jpg"  >

Ahora vamos a observar la configuración que nos da cuando arrastramos la opción Mediana con Cuartiles, esta opción nos mostrara la media por grupo (año) el cuartil inferior y superior  brindándonos una media de salarios, como se muestra en la siguiente imagen:

<img src="../images/05/25.jpg"  >

El resultado final es el siguiente:

<img src="../images/05/26.jpg"  >

Ahora vamos a conocer el análisis de tipo de modelo, para este desarrolla vamos a crear otra hoja que le llamaremos modelo y arrastraremos los campos años, nombre en el apartado de columnas y salario en la parte de filas como se muestra en la siguiente imagen:

<img src="../images/05/27.jpg"  >


Ahora colocados los datos solicitados vamos a formatear el apartado de nombre dando clic derecho sobre nombre y seleccionaremos la opción Formatear como se muestra a continuación:

<img src="../images/05/28.jpg"  >

Ahora formateado nuestros nombres, vamos a ir a nuestra pestaña de análisis y seleccionaremos la primer opción Promedio por intervalo de confianza, este promedio es el que nos ayuda a estimar un determinado nivel de confianza mediante un estudio obtenido o un rango obtenido sobre una media y su representación gráfica es la siguiente, para ellos seleccionaremos la opción a nivel de panel, como se muestra en la siguiente imagen:

<img src="../images/05/29.jpg"  >

Eliminamos nuestro ejemplo anterior y ahora nos vamos a análisis y arrastraremos la opción Media con intervalo de confianza, este análisis nos ayudara a estimar el grado de imprecisión de la estimación; es inversamente proporcional al tamaño de la muestra, la estimación se hace para un determinado nivel de confianza, usualmente 95% o 99% y para poder realizarla solo basta con arrastrar hacia nuestra gráfica y nos aparecerán las diferentes formas en la que la podemos representar para este ejemplo seleccionaremos la opción panel.

<img src="../images/05/30.jpg"  >

Ahora vamos a crear otra hoja de trabajo para trabajar las opciones de análisis a nivel tendencia para ellos nombraremos con ese nombre nuestra hoja, para este ejercicio será necesario arrastrar los campos Máximo salario a la parte de columnas y Mínimo Salario a la parte de Filas como se muestra en la imagen.

<img src="../images/05/31.jpg"  >

Ya con estos datos colocados en nuestra tabla de trabajo, nos iremos a nuestra tabla de análisis y antes de trabajar con las opciones de tendencia vamos a agregar también año en el apartado de detalles en nuestra caja de herramientas, como se muestra en la siguiente imagen.

<img src="../images/05/32.jpg"  >

Ahora si con este último ajuste nos vamos a nuestra pestaña de Análisis y observemos que tenemos disponible ya Línea de Tendencia, Pronostico y Clúster, vamos a iniciar con la opción de línea de tendencia arrastraremos nuestra opción al gráfico y seleccionaremos la opción de manera lineal como se muestra en la siguiente imagen:

<img src="../images/05/33.jpg"  >

Para nuestro siguiente ejercicio vamos a crear otra tabla de trabajo en la cual colocaremos el nombre de Pronostico, creada esta nueva hoja de trabajo, vamos a arrastrar el campo de Año a columnas y Salario a filas,  en la opción mostrar vamos a seleccionar el grafico de barras y lo colocaremos de manera Vertical como se muestra en la siguiente imagen:  

<img src="../images/05/34.jpg"  >


Realizado la anterior vamos a ir a nuestra opción de Análisis y arrastraremos la opción de pronósticos a nuestro grafico en automático nos aparecerá la opción pronostico ahí la soltaremos como mostramos en la siguiente imagen:

<img src="../images/05/35.jpg"  >

Al realizar lo anterior nos mostrar un pronóstico de salarios para el año 2008 y 2009 una potente herramienta para pronosticar ventas o comportamientos de mercado.

<img src="../images/05/36.jpg"  >

Ahora vamos a crear otra tabla de trabajo en la cual colocaremos el nombre a esta hoja como clúster, para este análisis vamos a arrastra Nombre a la parte de columnas y Salario a la parte de las filas como se muestra en la siguiente imagen:

<img src="../images/05/37.jpg"  >

Realizado lo anterior vamos a ir a nuestra pestaña de análisis y arrastraremos la opción de Clúster, lo que observamos al realizar esta configuración es que nos agrupara los valores en base al crecimiento para ellos vamos a ordenar de manera Ascendente nuestra información para obtener el resultado como muestra en la siguiente imagen: 

<img src="../images/05/38.jpg"  >

Ahora vamos a crear un análisis de tipo Personalizado para ello vamos a crear una nueva hoja de trabajo con este nombre PERSONALIZADO, para esta hoja vamos a arrastrar en la parte de columnas AÑO y NOMBRE en la parte de filas vamos arrastra SALARIO justo como se muestra en la siguiente imagen:

<img src="../images/05/39.jpg"  >

Echo lo anterior vamos a formatear el campo de nombre y colocaremos la alineación de texto de tipo normal para que nos quede nuestro grafico de la siguiente manera:

<img src="../images/05/40.jpg"  >

Realizado el formateo vamos a dirigirnos a nuestra pestaña de Análisis y vamos a arrastra la opción de línea de referencia que es igual que nuestras opciones de línea de constante y línea de promedio, vamos a arrastrarla y observemos que nos aparecen también las opciones de formateo como las líneas, nosotros vamos a seleccionar la parte de panel como se muestra en la siguiente imagen:

<img src="../images/05/41.jpg"  >

Al personalizar nuestra línea de referencia nos quedara nuestro grafico de la siguiente manera:

<img src="../images/05/42.jpg"  >

Ahora eliminemos la línea de referencia y arrastramos la opción de banda de referencia , lo arrastraremos a nivel de tabla y configuraremos como se muestra en la siguiente imagen:

<img src="../images/05/43.jpg"  >

El resultado de esa configuración es el siguiente, donde nos mostrara el máximo y la media del salario:

<img src="../images/05/44.jpg"  >

Ahora vamos a utilizar la opción de Banda de Distribución y aplicaremos la siguiente configuración como se muestra en la imagen:

<img src="../images/05/45.jpg"  >

El resultado final es el siguiente: 

<img src="../images/05/46.jpg"  >

Ahora vamos a revisar el Diagrama de Caja, para ello vamos a crear otra hoja de trabaja con el nombre de Diagrama y vamos a arrastrar en columna Año y en filas Salario, después vamos a ir a mostrar y seleccionaremos el grafico de líneas continuas.

<img src="../images/05/47.jpg"  >

Realizado lo anterior arrastramos desde nuestra pestaña de análisis la opción de Diagrama de caja y realizamos la siguiente configuración: 

<img src="../images/05/48.jpg"  >

El resultado final seria 

<img src="../images/05/49.jpg"  >

Ahora para este siguiente desarrollo, vamos nosotros a crear gráficos avanzados con los cuales nosotros configuraremos con una seria de combinaciones, para esto vamos a crear una nueva hoja y le colocaremos el nombre de Donas, creada esta nueva hoja vamos a arrastrar el campo Job Title en la parte de filas y Salarios en la parte de Datos como se muestra en la siguiente imagen:

<img src="../images/05/50.jpg"  >

Ahora en la parte de Mostrar vamos a establecer el Grafico Circular y después colocaremos la vista completa para obtener el siguiente resultado: 

<img src="../images/05/51.jpg"  >

Ahora vamos a dar doble clic sobre la parte de columnas y colocaremos le número 1 , después daremos clic nuevamente y colocaremos el numero 2 esto para crear 2 gráficos de pastel, realizada esta parte vamos a observar que en la parte de Marcas nos aparecen los 2 gráficos, editaremos el grafico 2 donde quitaremos el campo Job Title y Salario para que nos quede un círculo gris y en el grafico 1 solo aumentaremos el tamaño de este.

<img src="../images/05/52.jpg"  >

Ahora donde tenemos el 1 y 2 en columna daremos clic sobre cada uno y seleccionaremos la opción dimensión, ahora daremos clic sobre el eje 2 y seleccionaremos la opción que dije Eje Doble

<img src="../images/05/53.jpg"  >
Ahora vamos a dar clic sobre marcas y seleccionaremos el eje 2 en el cual personalizaremos su color de gris a blanco y adaptaremos su tamaño en lo posterior nos iremos a eje 1 y seleccionaremos mostrar etiquetas como se muestra en las siguientes imágenes:

<img src="../images/05/54.jpg"  >

Personalicemos más este grafico de pastel, vamos a desactivar las etiquetas y en el eje 1 vamos a arrastrar a el módulo de etiquetas el campo Job Title y en el eje 2 vamos arrastra a etiquetas el campo Salario dando como resultado las siguientes imágenes:

<img src="../images/05/55.png"  >

Ahora vamos a crear una nueva hoja y colocaremos como nombre porcentaje, vamos arrastra a la parte de columnas años, en la parte de filas salario, aplicaremos dentro de marcar en la parte de colores el Puesto (Job Title), 

<img src="../images/05/56.jpg"  >

Creado lo anterior es necesario formatear el salario a nivel porcentaje del total para ellos daremos clic sobre salario en la parte de columnas y seleccionaremos la opción de cálculo rápido y aplicaremos la opción de porcentaje en el Total.

<img src="../images/05/57.jpg"  >

Vamos a personalizar una más este grafico para ellos daremos clic de nuevo sobre salario y seleccionaremos la opción Calculo Usado y colocaremos la opción Tabla a lo Largo, posteriormente nos iremos a Marcas y en la parte de color seleccionaremos el límite y colocaremos líneas negras además activaremos las etiquetas para obtener el siguiente resultado: 

<img src="../images/05/58.jpg"  >

Ahora vamos a crear otro tipo de grafico para ellos colocaremos a una nueva hoja el nombre de Grafico Totales, vamos a arrastrar el campo Job Title en la parte de filas, también colocaremos Nombre y en la parte de filas colocaremos el salario: 

<img src="../images/05/59.jpg"  >

Ahora presionando la tecla control y arrastramos de columna la parte de salario, observaremos que nos va a crear una segunda columna con esa data, ahora en esa segunda columna daremos clic y seleccionaremos cálculo de trabajo rápido y seleccionaremos clasificación  

<img src="../images/05/60.jpg"  >

Ya que formateamos nuestra segunda columna de barras por clasificaciones, ahora vamos a dar de nuevo clic sobre el segundo campo valor de salario en columna y seleccionaremos calcular usando y después nombre, por último daremos de nuevo clic derecho a esta segunda columna y daremos clic en mostrar filtro, esto nos ayudara a activar un filtro de clasificación de salarios, realizado esto eliminaremos la segunda columna y observemos que podemos organizar nuestros valores dependiendo el número de clasificación de 1 hasta 5 o de 1 hasta 10.

<img src="../images/05/61.jpg"  >

El resultado después de eliminar la segunda columna de salario y aplicado el filtrado es el siguiente: 

<img src="../images/05/62.jpg"  >

Ahora vamos a crear otra hoja nueva de trabajo donde le colocaremos le nombre de Lollipop, aquí vamos a arrastra en la parte de filas el título de trabajo(Job Title), en columnas colocaremos Salario y con la tecla control arrastraremos nuestro campo de columnas salario para crear 2 columnas en nuestro grafico como se muestra a continuación:

<img src="../images/05/63.jpg"  >

Ahora en la segunda opción de salario daremos clic sobre él y seleccionaremos la opción Eje doble para que nos aparezca el siguiente resultado:

<img src="../images/05/64.jpg"  >

Realizado lo anterior observemos en la caja de nombre marcas nos aparecen varias casillas Todo, Sumada de salario 1 y Suma de salario 2, vamos a personaliza la segunda opción de Salario donde estableceremos en la lista desplegable donde dice Automático seleccionaremos la opción circulo y en la primera opción de salario en la misma lista desplegable seleccionaremos grafico de barra y obtendremos el siguiente resultado:

<img src="../images/05/65.jpg"  >

Realizado lo anterior vamos a realizar algunos ajustes a nuestra primera opción de salario dentro de la caja de Marcas, primero vamos a reducir un poco el tamaño hasta una línea atrás, después vamos a cambiar de color y colocaremos un límite ahí mismo en colores de color negro, ahora haremos lo mismo en la segunda opción de salario solo que aquí vamos a agrandar hasta una línea después y las demás modificaciones aplicaran igual con distinto color como se muestra en la siguiente imagen:

<img src="../images/05/66.jpg"  >

Realizado lo anterior el resultado será el siguiente:

<img src="../images/05/67.jpg"  >

Ahora vamos a crear una nueva hoja que le colocaremos de nombre World Cloud, aquí arrastraremos en filas lo Títulos de trabajo y en la parte de columnas colocaremos el Salario, ahora nos iremos a mostrar y seleccionaremos el grafico de mapa de calor como se muestra en la imagen:

<img src="../images/05/68.jpg"  >

Creado lo anterior vamos a irnos a nuestra caja de marcas y en la lista desplegable vamos a seleccionar la opción que dice Texto y nos cambiara totalmente nuestro grafico a los nombres de los puestos de trabajo en la parte del filtrado activado a mano derecha cambiaremos el color a rojo como se muestra en la siguiente imagen: 

<img src="../images/05/69.jpg"  >


Ahora vamos a crear otra hoja de trabajo que la nombraremos Línea Diferencial, para este grafico presionando la tecla Control vamos a seleccionar Job Title, Max Salary, Min Salary , así se quedaran señalados nos iremos a la herramienta de mostrar y seleccionaremos la opción de Tabla de Texto como se muestra en las siguientes imágenes:

<img src="../images/05/70.jpg"  >

Ahora si miramos bien creo medida en automático nuestro gráfico, para ello la medida que está en marcas vamos a arrastrarla a la parte de Columnas y la de Columnas la vamos a arrastrar a colores para que generar el siguiente grafico:

<img src="../images/05/71.jpg"  >

Ahora con la tecla control vamos a duplicar nuestra medida que está en la parte de columnas y a la segunda medida daremos clic y seleccionaremos eje doble, Ahora en la parte de marcas de nuevo nos activa Todo, Medida 1 y Medida 2, en la Medida 2 sobre la lista desplegable seleccionaremos la opción de líneas para que nos muestre el siguiente gráfico.

<img src="../images/05/72.jpg"  >

El resultado que obtendremos será un gráfico de línea, ahora vamos a ir a nuestra herramienta de Marcas y arrastraremos nombre de medida hacia la opción de ruta para obtener el siguiente grafico:

<img src="../images/05/73.jpg"  >

Ahora como ultimo toque vamos a ir a nuestro valor de medida 1 y vamos a modificar el tamaño un poco más grande, realizado esto vamos a dar clic derecho sobre el grafico y presionaremos la opción sincronizar eje y obtendremos el siguiente resultado:


<img src="../images/05/74.jpg"  >

Ahora vamos a crear otra hoja a la cual la nombraremos Barra dentro de Barra, aquí vamos a arrastrar el campo Country Name a filas y salario al campo de valores, en la parte de nuestra herramienta mostrar seleccionaremos el grafico de barra para obtener el siguiente resultado:

<img src="../images/05/75.jpg"  >

Realizado lo anterior, ahora vamos arrastra a colores el campo de año , echo eso vamos a dar clic sobre año y activaremos el filtrado por año como se muestra en la imagen: 

<img src="../images/05/76.jpg"  >

Ahora vamos a configurar las barras para ellos nos iremos al menú de análisis, iremos a la opción Apilar Marcas y lo desactivaremos,  ahora en nuestra herramienta de marcas con la letra control arrastraremos años y lo colocaremos sobre la opción de tamaño y nos mostrara el siguiente grafico:

<img src="../images/05/77.jpg"  >

Ahora vamos a crear nuestro ultimo grafico avanzado y nombraremos a esta hoja como Barra de Colores – Unicode, vamos a arrastrar el campo de Job Title, Nombre  a la parte de filas  y salario a la parte de Datos.


<img src="../images/05/78.jpg"  >

Ahora en nuestra herramienta de mostrar vamos a seleccionar grafico en barra y este lo configuraremos de forma Descendente

<img src="../images/05/79.jpg"  >
Ahora con la tecla control vamos a selecciona Job Title y Nombre para crear una dimensión y los arrastraremos a la opción de colores.

<img src="../images/05/80.jpg"  >

Ahora vamos a personalizar vamos a invertir las cosas de nuestra medida dentro de Marcas subiremos Job Title y abajo quedara nombre a demás colocaremos la opción de marcas como se muestra en la siguiente imagen:

<img src="../images/05/81.jpg"  >

Ahora vamos a crear un código que nos ayude a crear un top de los mejores salarios y que le ponga una imagen a cada uno de ellos para ello iremos al siguiente web site que utilizaremos para estas imágenes:
http://xahlee.info/comp/unicode_circled_numbers.html

<img src="../images/05/82.jpg"  >

Ya en sitio web vamos a necesitar los numero del 1 al 3, pero antes de hacer eso vamos a ir de nuevo a nuestro Tableau y realizaremos la siguiente programación y para ellos crearemos un campo calculado dando clic sobre la pestaña que está al lado de buscar dentro de nuestra data,

<img src="../images/05/83.jpg"  >

*OJO:* Colocaremos los números del sitio web entre comillas doble en nuestra instrucción que programamos.

Ahora creado este campo calculado vamos a arrastrarlo al campo etiquetas dentro de nuestra herramienta Marcas:

<img src="../images/05/84.jpg"  >

También nosotros podemos programar nuestro top por título de trabajo para ellos iremos a nuestra herramienta de Marcas y daremos clic cobre Unicode, aquí seleccionaremos editar cálculo de tabla y nos aparecerá un cuadro de dialogo donde activaremos A nivel más Profundo y la opción de reiniciado cada seleccionaremos Job Title

<img src="../images/05/85.jpg"  >

### Tarea 2. Práctica Libre

Objetivo: Desarrollar un dashboard de control que permita a los usuarios visualizar y analizar datos de manera eficiente, utilizando diversas funcionalidades de Tableau como filtros, gráficos dinámicos, y acciones interactivas. El objetivo es que los participantes adquieran habilidades prácticas en la creación de dashboards que faciliten la toma de decisiones basada en datos, aplicando buenas prácticas de diseño y usabilidad.
Instrucción: En base a lo aprendida hasta el momento es necesario realizar un dashboard donde combinemos las diferentes gráficas, tablas, filtros, colores que nos ayude a transmitir la historia que nuestro data set está trasmitiendo:
1.- Utilizarás las bases de datos que se te proporcionaran.
2.- Este Dashboard debe de ser lo más parecido a la imagen 

<img src="../images/05/86.jpg"  >
