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

Para este desarrollo es necesario descargar la data de la carpeta **Segundo Proyecto**.

Para continuar con el proyecto, tienes que crear una carpeta y descargar el archivo `Data.zip`; una vez descargado, extrae sus archivos, los cuales tienen los siguientes nombres:

*Crear Carpeta -> "Dashboard - Recursos Humanos"*
*Data.xlsx*
*ESQUEMA_RRHH.jpg*
*Background.jpg*


Con la data en el escritorio, analiza el archivo tomando como base este diagrama: 

<img src="../images/05/01.jpg"  >


Una vez explicado el desarrollo y las relaciones necesarias, iniciar tu proyecto.

Para ello, carga el archivo de Excel de nombre `Data` seleccionando el tipo de formato de archivo que utilizarás.

<img src="../images/05/02.jpg"  >

Con la data cargada, aparecerá de la siguiente manera.

<img src="../images/05/03.jpg"  >

Lo primero que colocarás es la tabla de `Empleados` (`Employee`) y arrastra también la de `Trabajo` (`job`). Estas se relacionarán con el campo `JOB ID`.

<img src="../images/05/04.jpg"  >

Ahora, arrastra el campo `Historial de trabajos` (`job_History`) y relaciónalo con la tabla de `Trabajo` ambos por el campo `JOB ID`.

<img src="../images/05/05.jpg"  >

Arrastra la tabla `Departamento` (`Department`) y relaciónala con la tabla de `Empleados`, ambos por el campo `Departmen ID`.

<img src="../images/05/06.jpg"  >


Arrastra la tabla `Ubicaciones` (`Locations`) y relaciónala con la tabla de `Departamento`, ambas por el campo `Location ID`.

<img src="../images/05/07.jpg"  >

Arrastra la tabla `Estado` (`Countries`) y relaciónala con la tabla de `Ubicaciones`, ambas por el campo `Country ID`.

<img src="../images/05/08.jpg"  >

Finalmente, arrastra la tabla `Region` y relaciónala con la tabla de `Estado`, ambas por el campo `Region ID`.

<img src="../images/05/09.jpg"  >

El resultado final de la data es el siguiente: 

<img src="../images/05/10.jpg"  >

Para darle una mejor estructura al modelo de datos, ve tabla por tabla y oculta los campos innecesarios para el manejo de datos, estos campos solo ayudarían a relacionar y crear el modelo.

Estos campos serán todos los ID de las tablas como se muestra en la imagen:

<img src="../images/05/11.jpg"  >

Ya que ocultaste estos campos innecesarios para el desarrollo, da clic sobre la `Hoja 1` y aparecerán  los datos de la siguiente manera.

<img src="../images/05/12.jpg"  >

Prueba que está todo bien; para ello, en filas, coloca el campo `First Name` y como dato coloca el campo `Salary` para que presente el siguiente listado:

<img src="../images/05/13.jpg"  >

Ahora, crea un campo calculado donde unas el campo `First Name` más el campo `Last Name` de la siguiente manera.

<img src="../images/05/14.jpg"  >

Ya que validaste que todo está en orden, remueve los datos anteriores de la tabla de trabajo y arrastra  el campo `Hire Date` (`Fecha de Contratacion`) y `Nombre` en columnas y en las filas coloca  el campo `Salary`.
Una vez hecho, presiona en formatear sobre `Nombre` y coloca los nombres centrados de manera horizontal como se muestra en la siguiente imagen.

<img src="../images/05/15.jpg"  >

Creado el grafico de salarios, ve a la pestaña `Análisis`, para conocer más de esta herramienta.

| Herramienta  | Función |
| ------------- | ------------- |
| Pestaña de análisis  | Herramienta para explorar patrones, tendencias y detalles en datos. |
| Arrastrar y soltar objetos analíticos | Líneas, bandas, áreas, totales → destacan aspectos clave.  |
| Líneas de referencia  | Promedios, medianas, mínimos o máximos → contextualizan datos.  |
| Barras de referencia  | Marcan rangos o límites específicos en la visualización. |
| Líneas de tendencia  | Muestran comportamiento en el tiempo o frente a otra variable (lineal, exponencial, logarítmico). |
| Previsiones | Proyectan tendencias futuras con base en datos históricos. |
| Cálculos rápidos de tabla  | Porcentajes, diferencias, totales → aplicados desde la pestaña `Análisis`.  |
| Resaltado | Reglas para identificar valores atípicos o áreas de interés.  |
| Agrupación y clústeres  | Grupos automáticos según las similitudes en los datos.  |

Suelta y observa que se solicita un valor; para este ejemplo, coloca  $12,000  que será la línea constante, esta sirve para analizar los datos que sobrepasen este tope de valor, es por ello que a lo largo del gráfico debes colocar una línea horizontal con un valor de 12,000.

<img src="../images/05/16.jpg"  >

Esta constante también se puede formatear si tuvieras la necesidad de cambiar el valor hasta personalizar la línea dando clic; sobre él, aparecerá un menú donde puedes acceder a estos ajustes como se muestra en la siguiente imagen.

<img src="../images/05/17.jpg"  >

Da clic sobre la opción `Formatear`; en esta opción, puedes personalizar la línea desde la forma, color y grosor, como se muestra en la siguiente imagen. 

<img src="../images/05/18.jpg"  >

Ahora ve de nuevo a la pestaña de análisis y arrastra la opción de `Línea de Promedio`; aparecerá una opción donde debes especificar la línea de referencia que tomarás como se muestra en la siguiente imagen, donde seleccionarás como tabla: 

<img src="../images/05/19.jpg"  >

Si observas, aparece una línea igual de constante, solo que aquí señala el promedio de salarios que se tienen.

<img src="../images/05/20.jpg"  >

Ahora elimina la línea de nuevo. Dirígete a la pestaña de análisis, selecciona `Línea de Promedio` y la opción de `Panel` como se muestra en la imagen:

<img src="../images/05/21.jpg"  >

Ahora, esta opción muestra los promedios por panel por cada sección como se muestra en la imagen:

<img src="../images/05/22.jpg"  >

De nuevo, elimina la línea y ve por la última opción en línea de referencia, pero esta vez por celda:

<img src="../images/05/23.jpg"  >

Justo esta opción te ayudará a ver el promedio por cada una de las celdas o columnas para realizar una visión de crecimiento más adecuada, como se muestra en la imagen.

<img src="../images/05/24.jpg"  >

Ahora, observa la configuración dada cuando arrastra la opción `Mediana con Cuartiles`, esta opción mostrará la media por grupo (año) el cuartil inferior y superior para brindar una media de salarios, como se muestra en la siguiente imagen.

<img src="../images/05/25.jpg"  >

El resultado final es el siguiente:

<img src="../images/05/26.jpg"  >

Ahora, conocerás el análisis de tipo de modelo, para este desarrollo crearás otra hoja a la que llamarás modelo y arrastrarás los campos años, nombre en el apartado de columnas y salario en la parte de filas como se muestra en la siguiente imagen.

<img src="../images/05/27.jpg"  >


Ahora colocados los datos solicitados, formatea el apartado de nombre dando clic derecho sobre nombre y selecciona la opción `Formatear` como se muestra a continuación.

<img src="../images/05/28.jpg"  >

Ahora formateados los nombres, ve a la pestaña de análisis y selecciona la primera opción `Promedio por intervalo de confianza`, este promedio ayuda a estimar un determinado nivel de confianza mediante un estudio obtenido o un rango obtenido sobre una media y su representación gráfica es la siguiente; para ello, selecciona  la opción a nivel de panel, como se muestra en la siguiente imagen.

<img src="../images/05/29.jpg"  >

Elimina el ejemplo anterior y ahora realiza un análisis: arrastra la opción `Media con intervalo de confianza`. Este análisis ayudará a estimar el grado de imprecisión de la estimación; es inversamente proporcional al tamaño de la muestra. La estimación se hace para un determinado nivel de confianza, usualmente 95 o 99 % y para poder realizarla solo basta con arrastrar hacia la gráfica y aparecerán las diferentes formas en la que la puedes representar. Para este ejemplo, selecciona  la opción panel.

<img src="../images/05/30.jpg"  >

Ahora, crea otra hoja de trabajo para trabajar las opciones de análisis a nivel tendencia; para ello, nombra la hoja. Para este ejercicio, será necesario arrastrar los campos `Salario Máximo` a la parte de columnas y `Salario Mínimo` a la parte de Filas como se muestra en la imagen.

<img src="../images/05/31.jpg"  >

Ya con estos datos colocados en la tabla de trabajo, ve a la tabla de análisis y antes de trabajar con las opciones de tendencia agrega también el año en el apartado de detalles en la caja de herramientas, como se muestra en la siguiente imagen.

<img src="../images/05/32.jpg"  >

Con este último ajuste, la pestaña de `Análisis` y observa que tienes disponible ya la `Línea de Tendencia`, `Pronóstico` y `Clúster`; inicia con la opción de línea de tendencia, arrastra la opción al gráfico y selecciona la opción de manera lineal como se muestra en la siguiente imagen.

<img src="../images/05/33.jpg"  >

Para el siguiente ejercicio, crea otra tabla de trabajo para colocar el nombre de `Pronóstico`, creada esta nueva hoja de trabajo, arrastra el campo de `Año a columnas` y `Salario a filas`. En la opción `Mostrar`, selecciona el grafico de barras y lo coloca  de manera Vertical como se muestra en la siguiente imagen.  

<img src="../images/05/34.jpg"  >


Una vez hecho la anterior ir a la opción de `Análisis` y arrastra  la opción de pronósticos al gráfico en automático aparecerá la opción pronostico, ahí suéltala  como se muestra en la siguiente imagen.

<img src="../images/05/35.jpg"  >

Al realizar lo anterior, mostrará un pronóstico de salarios para el año 2008 y 2009 una potente herramienta para pronosticar ventas o comportamientos de mercado.

<img src="../images/05/36.jpg"  >

Ahora, crea otra tabla de trabajo. Nombra esta hoja como clúster; para este análisis, arrastra `Nombre` a la parte de columnas y `Salario` a la parte de las filas como se muestra en la siguiente imagen.

<img src="../images/05/37.jpg"  >

Una vez hecho lo anterior, ve a la pestaña de `Análisis` y arrastra la opción de `Clúster`. Lo que observas al realizar esta configuración es que agrupará los valores en base al crecimiento; para ello ordena de manera ascendente la información para obtener el resultado como muestra en la siguiente imagen. 

<img src="../images/05/38.jpg"  >

Ahora, crea un análisis de tipo `Personalizado`; para ello, crea una nueva hoja de trabajo con el nombre `PERSONALIZADO`; para esta hoja, arrastra a la parte de columnas `AÑO` y `NOMBRE`; en la parte de filas, arrastra `SALARIO` justo como se muestra en la siguiente imagen.

<img src="../images/05/39.jpg"  >

Hecho lo anterior, formatea el campo de nombre y coloca la alineación de texto de tipo normal para que quede el gráfico de la siguiente manera.

<img src="../images/05/40.jpg"  >

Una vez hecho el formateo, dirígete a la pestaña de `Análisis` y arrastra la opción de línea de referencia que es igual que las opciones de línea de constante y línea de promedio, arrástrala y observa que aparecen también las opciones de formateo como las líneas. Selecciona la parte de panel como se muestra en la siguiente imagen.

<img src="../images/05/41.jpg"  >

Al personalizar la línea de referencia, quedará el gráfico de la siguiente manera.

<img src="../images/05/42.jpg"  >

Ahora, elimina la línea de referencia y arrastra la opción de banda de referencia , arrástralo a nivel de tabla y configúralo como se muestra en la siguiente imagen.

<img src="../images/05/43.jpg"  >

El resultado de esa configuración es el siguiente, donde mostrará el máximo y la media del salario:

<img src="../images/05/44.jpg"  >

Ahora, utiliza la opción de `Banda de Distribución` y aplica la siguiente configuración como se muestra en la imagen.

<img src="../images/05/45.jpg"  >

El resultado final es el siguiente.

<img src="../images/05/46.jpg"  >

Ahora, revisa el Diagrama de Caja. Para ello, crea otra hoja de trabajo con el nombre de `Diagrama` y arrastra a la columna `Año` y en la fila `Salario`, después ve a `Show` y selecciona el gráfico de líneas continuas.

<img src="../images/05/47.jpg"  >

Una vez hecho lo anterior, arrastra desde la pestaña de análisis la opción de `Diagrama de caja` y realiza la siguiente configuración.

<img src="../images/05/48.jpg"  >

El resultado final sería:

<img src="../images/05/49.jpg"  >

Ahora, para este siguiente desarrollo, crearás gráficos avanzados con los cuales configurarás una seria de combinaciones. Para esto, crea una nueva hoja y con el nombre de `Donas`; creada esta nueva hoja, arrastra el campo `Job Title` en la parte de filas y `Salarios` en la parte de `Datos` como se muestra en la siguiente imagen.

<img src="../images/05/50.jpg"  >

Ahora, en la parte de `Mostrar` establece el Gráfico Circular y después coloca la vista completa para obtener el siguiente resultado.

<img src="../images/05/51.jpg"  >

Ahora, da doble clic sobre la parte de columnas y colócale número 1 , después da clic nuevamente y coloca el número 2; esto para crear dos gráficos de pastel.  Luego, observa que en la parte de `Marcas` aparecen los dos gráficos, edita  el gráfico 2, quita el campo `Job Title` y `Salario` para que quede un círculo gris y en el gráfico 1 solo aumenta su tamaño.

<img src="../images/05/52.jpg"  >

Ahora, donde está el 1 y 2 en la columna da clic sobre cada uno y selecciona la opción dimensión. Ahora, da clic sobre el eje 2 y selecciona la opción `Eje Doble`.

<img src="../images/05/53.jpg"  >
Ahora da clic sobre `marcas` y selecciona  el eje 2. Personaliza su color de gris a blanco y adapta su tamaño en lo posterior. Ve al eje 1 y selecciona `mostrar etiquetas` como se muestra en las siguientes imágenes.

<img src="../images/05/54.jpg"  >

Personaliza más este gráfico de pastel: desactiva las etiquetas y en el eje 1, arrastra al módulo de etiquetas el campo `Job Title` y en el eje 2 arrastra las etiquetas al campo `Salario` dando como resultado las siguientes imágenes.

<img src="../images/05/55.png"  >

Ahora, crea una nueva hoja y coloca como nombre `porcentaje`, arrastra a la parte de columnas `años`, en la parte de filas `Salario` y aplica dentro de marcar en la parte de colores el `Puesto` (`Job Title`), 

<img src="../images/05/56.jpg"  >

Ahora, formatea el salario a nivel porcentaje del total; para ello, da clic sobre `salario` en la parte de columnas y selecciona  la opción de cálculo rápido y aplica la opción de porcentaje en el `Total`.

<img src="../images/05/57.jpg"  >

Para personalizar más este grafico, da clic de nuevo sobre `Salario` y selecciona la opción `Cálculo Usado` y coloca la opción `Tabla a lo Largo`, posteriormente dirígete a `Marcas` y en la parte de color, selecciona el límite y coloca líneas negras; además, activa las etiquetas para obtener el siguiente resultado.

<img src="../images/05/58.jpg"  >

Ahora, crea otro tipo de gráfico; para ello coloca una nueva hoja el nombre de `Gráfico Totales`, arrastrar el campo `Job Title` en la parte de filas, también coloca `Nombre` y en la parte de filas coloca el salario.

<img src="../images/05/59.jpg"  >

Ahora, presionando la tecla control, arrastra de columna la parte de salario. Observa que se creará una segunda columna con esa data. Ahora, en esa segunda columna, da clic y selecciona `cálculo de trabajo rápido` y `clasificación`. 

<img src="../images/05/60.jpg"  >

Ya que formateaste la segunda columna de barras por clasificaciones. Ahora, da clic de nuevo sobre el segundo campo valor de `Salario` en columna y selecciona  `calcular` y después `Nombre`, por último, da clic derecho a esta segunda columna y en mostrar filtro. Esto ayudará a activar un filtro de clasificación de salarios. Luego, elimina la segunda columna y observa que puedes organizar los valores dependiendo el número de clasificación de 1 hasta 5 o de 1 hasta 10.

<img src="../images/05/61.jpg"  >

El resultado después de eliminar la segunda columna de salario y aplicado el filtrado es el siguiente.

<img src="../images/05/62.jpg"  >

Ahora, crea otra hoja nueva de trabajo con el nombre de `Lollipop`, aquí arrastra en las filas el título de trabajo (`Job Title`). En columnas, coloca `Salario` y con la tecla control arrastra el campo de columnas `Salario` para crear dos columnas en el gráfico como se muestra a continuación.

<img src="../images/05/63.jpg"  >

Ahora en la segunda opción de salario da clic sobre él y selecciona  la opción Eje doble para que aparezca el siguiente resultado.

<img src="../images/05/64.jpg"  >

Ahora, observa en la caja de nombre las marcas que aparecen en varias casillas: `Todo`, `Suma de salario 1` y `Suma de salario 2`, personaliza la segunda opción de `Salario`. En la lista desplegable `Automático`, selecciona la opción círculo y en la primera opción de salario en la misma lista desplegable selecciona `Gráfico de barra` para obtener el siguiente resultado.

<img src="../images/05/65.jpg"  >

Luego, realiza algunos ajustes a la primera opción de salario dentro de la caja de `Marcas`, primero reduce un poco el tamaño hasta una línea atrás, después cambia el color y coloca un límite ahí mismo en colores de color negro. Ahora haz lo mismo en la segunda opción de salario, solo que aquí agranda hasta una línea después y las demás modificaciones se aplicarán igual con distinto color como se muestra en la siguiente imagen.

<img src="../images/05/66.jpg"  >

El resultado será el siguiente.

<img src="../images/05/67.jpg"  >

Ahora, crea una nueva hoja con el nombre `World Cloud`, aquí arrastra las filas los `Títulos de trabajo` y en la parte de columnas coloca el `Salario`. Dirígete a `mostrar` y selecciona el gráfico de mapa de calor como se muestra en la imagen.

<img src="../images/05/68.jpg"  >

Ahora, dirígete a la caja de marcas y, en la lista desplegable, selecciona la opción `Texto` y el gráfico cambiará totalmente los nombres de los puestos de trabajo. En la parte del filtrado activado, a mano derecha, cambia el color a rojo como se muestra en la siguiente imagen. 

<img src="../images/05/69.jpg"  >


Ahora, crea otra hoja de trabajo como `Línea Diferencial`. Para este gráfico, presiona la tecla `Control`, selecciona `Job Title`, Max `Salary`, Min `Salary` , así se quedarán señalados. Dirígete a la herramienta de `mostrar` y selecciona la opción de `Tabla de Texto` como se muestra en las siguientes imágenes.

<img src="../images/05/70.jpg"  >

Ahora, para que el gráfico cree una medida en automático, arrastra la medida que está en marcas a la parte de `Columnas` y la de Columnas a colores para que genere el siguiente gráfico.

<img src="../images/05/71.jpg"  >

Con la tecla `control`, duplica la medida que está en la parte de columnas y en la segunda medida da clic y selecciona eje doble. En la parte de marcas, de nuevo, activa `Todo`, `Medida 1` y `Medida 2`-, en la `Medida 2`, sobre la lista desplegable, selecciona la opción de líneas para que muestre el siguiente gráfico.

<img src="../images/05/72.jpg"  >

El resultado que obtendrás será un gráfico de línea. Ahora dirígete la herramienta `Marcas` y arrastra el nombre de medida hacia la opción de ruta para obtener el siguiente gráfico.

<img src="../images/05/73.jpg"  >

Como último toque, dirígete al valor de `medida 1` y modifica el tamaño un poco más grande. Una vez hecho esto, da clic derecho sobre el gráfico y presiona la opción `sincronizar eje`; obtendrás el siguiente resultado.


<img src="../images/05/74.jpg"  >

Luego, crea otra hoja con el nombre `Barra dentro de Barra`, aquí arrastra el campo `Country Name` a filas y `salario` al campo de valores, en la parte de la herramienta `mostrar`, selecciona el gráfico de barra para obtener el siguiente resultado.

<img src="../images/05/75.jpg"  >

Ahora, arrastra a `colores` el campo de año. Hecho esto, da clic sobre `año` y activa el filtrado por año como se muestra en la imagen.

<img src="../images/05/76.jpg"  >

Configura las barras: en el menú de `Análisis`, dirígete a la opción `Apilar Marcas` y  desactívalo. Ahora, en la herramienta de marcas con `Control`, arrastra `años` y colócalo sobre la opción de tamaño y mostrará el siguiente gráfico.

<img src="../images/05/77.jpg"  >

Crea el último gráfico avanzado y nombra esta hoja como `Barra de Colores – Unicode`, arrastra el campo de `Job Title`, `Nombre` a la parte de filas y `Salario` a la parte de `Datos`.


<img src="../images/05/78.jpg"  >

En la herramienta de `mostrar`, selecciona `gráfico en barra` y este configúralo de forma `Descendente`.

<img src="../images/05/79.jpg"  >
Con la tecla `control`, selecciona `Job Title` y `Nombre` para crear una dimensión y arrástralos a la opción de colores.

<img src="../images/05/80.jpg"  >

Ahora personaliza la disposición de los elementos dentro de la herramienta `Marcas`: coloca el campo `Job Title` en la parte superior y el Nombre debajo. Además, incluye la opción de `Marcas` tal como se muestra en la imagen.

<img src="../images/05/81.jpg"  >

Crea un código que ayude a crear un top de los mejores salarios y que le ponga una imagen a cada uno de ellos; para ello, dirígete al siguiente sitio web: 
http://xahlee.info/comp/unicode_circled_numbers.html

<img src="../images/05/82.jpg"  >

En el sitio, utiliza los números del 1 al 3. Antes de eso, regresa a Tableau y crea un campo calculado haciendo clic en la pestaña ubicada junto al buscador dentro de la data:

<img src="../images/05/83.jpg"  >

Importante. Coloca los números obtenidos del sitio web entre comillas dobles dentro de la instrucción que programes.

Una vez creado el campo calculado, arrástralo al área de `Etiquetas` dentro de la herramienta `Marcas`:

<img src="../images/05/84.jpg"  >

También puedes programar el Top por título de trabajo. Para ello, dirígete a la herramienta `Marcas`, haz clic sobre `Unicode`, selecciona `Editar cálculo de tabla` y, en el cuadro de diálogo que aparece, activa la opción `A nivel más profundo` y `Reiniciado cada`, seleccionando `Job Title`:

<img src="../images/05/85.jpg"  >

### Tarea 2. Práctica Libre

Desarrolla un dashboard de control que permita a los usuarios visualizar y analizar datos de manera eficiente, utilizando funcionalidades de Tableau como filtros, gráficos dinámicos y acciones interactivas. El objetivo es que los participantes adquieran habilidades prácticas en la creación de dashboards que faciliten la toma de decisiones basada en datos, aplicando buenas prácticas de diseño y usabilidad.

Con base en lo aprendido hasta el momento, crea un dashboard que combine diferentes gráficas, tablas, filtros y colores, transmitiendo la historia que el dataset refleja:
- Utiliza las bases de datos proporcionadas.
- El dashboard debe parecerse lo más posible a la imagen: 

<img src="../images/05/86.jpg"  >
