# Práctica 4. Dashboards e historias

## Objetivos
Al finalizar la práctica, serás capaz de:
- Diseñar dashboards efectivos.
- Añadir interactividad a los dashboards.
- Crear historias en Tableau.


## Objetivo visual 

<img src="../images/04/00.png" width="500" >



## Duración estimada
- 60 minutos.


## Instrucciones 

### Tarea 1. Crear un dashboard para mostrar información.

Has creado cuatro hojas de trabajo y están transmitiendo información importante que tu jefa debe conocer. Ahora necesitas una forma de mostrar las ganancias negativas en Tennessee, Carolina del Norte y Florida y explicar algunas de las razones por las que las ganancias son bajas.

Para hacerlo, puede utilizar dashboards para mostrar varias hojas de trabajo a la vez y, si lo desea, hacer que interaccionen entre sí.

#### Configurar el dashboard


1. Haz clic en el botón Nuevo dashboard.

<img src="../images/04/01.png" width="500" >

2. En el panel ``Dashboard`` de la izquierda, verá las hojas que creó. Arrastre ``Sales` in the South` a su dashboard vacío.

3. Arrastre ``Profit` Map` al dashboard y suéltelo encima de la vista ``Sales` in the South`.

La vista se actualizará para tener este aspecto:

<img src="../images/04/02.png" width="500" >

Ahora se pueden ver las dos vistas a la vez.

Lo malo es que el gráfico de barras tiene un aspecto confuso, lo cual no ayuda a que tu jefa comprenda los datos.

#### Organizar el dashboard

No resulta fácil ver los detalles de cada elemento de `Subcategoría` desde el gráfico de barras ``Sales` in the South` (Ventas del sur). Además, como tenemos el mapa en la vista, probablemente tampoco necesitemos la columna de la región South (Sur) en ``Sales` in the South` (Ventas del sur).

La resolución de estos problemas le aportará más espacio para poder transmitir la información que necesita.

1. En ``Sales` in the South` (Ventas del sur), haga clic con el botón derecho en el área de la columna situada debajo del encabezado de columna `Región` y desmarque Mostrar encabezado.

<img src="../images/04/03.png" width="300" >

2. Repite este proceso para el encabezado de filas `Categoría`.

<img src="../images/04/04.png" width="300" >

Ahora ha ocultado del dashboard las columnas y filas que no necesita, a la vez que conserva el desglose de los datos. El espacio adicional hace que sea más fácil ver los datos en su dashboard, pero mejoremos las cosas aún más.

3. Haz clic con el botón derecho en el título ``Profit` Map` y seleccione Ocultar título.

El título ``Profit` Map` desaparece del dashboard, lo que aporta más espacio.

3. Repite este paso para el título de la vista ``Sales` in the South` (Ventas del sur).

5. Selecciona la primera tarjeta de filtro `Subcategoría` a la derecha de la vista y, en la parte superior de la tarjeta, haga clic en el icono Eliminar ( <img src="../images/04/05.png" > ).

6. Repite este paso para la segunda tarjeta de filtro `Subcategoría` y para una de las tarjetas de filtro Año de fecha de pedido.

7. Haz clic en la leyenda de color de `Ganancias` y arrástrela desde el extremo derecho al extremo inferior de ``Sales` in the South` (Ventas del sur).

8. Por último, seleccione el filtro Año de fecha de pedido restante, haga clic en la flecha desplegable correspondiente y seleccione Flotante. Colóquelo en el espacio blanco de la vista de mapa. En este ejemplo está colocado en el lado de la costa este, en el océano Atlántico.

Intente seleccionar años distintos en el filtro `Year of Order Date`. Los datos se filtran rápidamente para mostrar que el rendimiento del estado varía según el año. Así está bien, pero podríamos cambiarlo para que sea más fácil compararlo.

9. Haz clic en la flecha desplegable de la parte superior del filtro `Year of Order Date` y seleccione Valor individual (barra deslizante).

La vista se actualiza y tiene más o menos este aspecto: 

<img src="../images/04/06.png" width="600" >

#### Diferenciar objetos flotantes frente a objetos en mosaico en un dashboard

Los objetos de un dashboard se pueden establecer en Mosaico o Flotante.

Los elementos en mosaico cambian de tamaño automáticamente para adaptarse a la zona donde son arrastrados. Los elementos flotantes se pueden mover y cambiar de tamaño libremente desde otros objetos del dashboard. Si lo desea, puede incluso tener elementos flotantes y en mosaico en el mismo dashboard.

¡Ahora su dashboard tiene un aspecto espectacular! Ahora puede comparar fácilmente las ganancias y las ventas por año. Se parece bastante a un par de imágenes en una presentación de diapositivas, ¡y estamos utilizando Tableau! Hagamos que su dashboard sea más atractivo

#### Compruebe su trabajo. Vea "Organizar el dashboard" en acción

<img src="../images/04/07.gif" width="800" >

#### Añadir interactividad

¿No sería genial si pudiera ver qué subcategorías son rentables en determinados estados?

1. Selecciona ``Profit` Map` en el dashboard y haga clic en el icono Usar como filtro (<img src="../images/04/08.png">), situado en la esquina superior derecha.

2. Selecciona un estado dentro de la región sur del mapa.

El gráfico de barras ``Sales` in the South` (Ventas del sur) se actualiza automáticamente y muestra solo las ventas por subcategoría del estado seleccionado. De esta manera, puede ver de un vistazo qué subcategorías son rentables.

3. Haz clic en un área del mapa que no sean los estados del sur coloreados para borrar tu selección.

También es recomendable que los lectores puedan ver el cambio en ganancias según la fecha del pedido.

4. Selecciona el filtro Año de fecha de pedido, haga clic en la flecha desplegable correspondiente y seleccione Aplicar a las hojas de trabajo > Hojas de trabajo seleccionadas.

5. En el cuadro de diálogo Aplicar filtro a las hojas de trabajo, seleccione Todo en el dashboard y, a continuación, haga clic en Aceptar.

Esta opción indica a Tableau que aplique el filtro a todas las hojas de trabajo del dashboard que utilicen la misma fuente de datos

Explore el rendimiento del estado según el año con el nuevo dashboard interactivo.

#### Compruebe su trabajo. Vea "Agregar interactividad" en acción

En este ejemplo filtramos ``Sales` in the South` (Ventas del sur) para que solo se muestren los artículos vendidos en North Carolina y exploramos las ganancias año por año.

<img src="../images/04/09.gif" width="800" >

#### Cambiar nombre y listo

Cuando muestra el dashboard a tu jefa, le encanta. Lo llama "Ventas regionales y ganancias" y tú hace lo mismo haciendo doble clic en la pestaña ``Dashboard`` 1 y escribiendo Ventas regionales y ganancias.

En sus investigaciones, tu jefa también detecta que la decisión de introducir máquinas en el mercado de North Carolina en 2021 fue una mala idea.

Su jefa se alegra de tener este dashboard con el que poder explorar la información, pero además le pide que presente un plan de acción claro al resto del equipo. Ella le pide que cree una presentación con tus hallazgos.

Menos mal que conoces las historias de Tableau.


### Tarea 2. Crear una historia para presentarla.

Quieres compartir tus hallazgos con el resto del equipo. Es posible que, juntos, reconsideren la venta de ``Machines`` en North Carolina.

En lugar de tener que adivinar qué información útil le interesa al equipo e incluirla en una presentación, decide crear una historia en Tableau. De este modo, puede explicar a los miembros del equipo el proceso con el que ha descubierto los datos y tendrá la opción de explorar interactivamente los datos para responder a cualquier pregunta que le planteen durante la presentación.

#### Crear el primer punto de la historia

Para la presentación, empezará con una introducción.

1. Haz clic en el botón Nueva historia.

<img src="../images/04/10.png" width="400" >

Se muestra un espacio con el siguiente mensaje: "Arrastre una hoja aquí". Aquí creará el primer punto de la historia.

Las historias en blanco se parecen mucho a los dashboards en blanco. Y como un dashboard, puede arrastrar hojas de trabajo para presentarlas. También puede arrastrar dashboards para presentarlos en la historia.

2. En el panel `Historia`, arrastre la hoja de trabajo ``Sales` in the South` a la vista.

3. Agrega un subtítulo, como "`Sales` and profit by year". Para hacerlo, edite el texto en el cuadro gris situado sobre la hoja de trabajo.

<img src="../images/04/11.png" width="700" >

Este punto de la historia será una forma útil de poner al corriente a los asistentes.

Pero quiere contar una historia sobre la venta de ``Machines`` en North Carolina, así que es el momento centrarse en esos datos.

#### Resaltar las ventas de ``Machines``

Para llegar hasta ``Machines``, puede aprovechar el filtro `Sub-Category` que se incluye en el gráfico de barras ``Sales` in the South`.

1. En el panel `Historia`, haga clic en Duplicar para duplicar el primer subtítulo.

Siga trabajando donde lo dejó, pero no olvide que el primer punto de la historia será exactamente como lo dejó.

2. Puesto que sabe que va a contar una historia sobre ``Machines``, en el filtro `Sub-Category`, desactive la selección para (Todos) y seleccione ``Machines``.

Ahora los asistentes pueden identificar rápidamente las ventas y las ganancias de ``Machines`` por año.

3. Agrega un subtítulo para destacar lo que ven los asistentes, como por ejemplo "Machine sales and profit by year".

<img src="../images/04/12.png" width="600" >

Ha cambiado el foco hacia ``Machines`` de manera adecuada, pero se da cuenta de que algo resulta extraño: En esta vista, puede identificar qué estado es el que más contribuye a la pérdida.

Solucionará esto en el siguiente punto de la historia mediante la introducción del mapa.

####  ¿Qué es esta barra de herramientas pequeña que aparece bajo el subtítulo del punto de la historia?

La barra de herramientas `Historia` <img src="../images/04/20.png"> aparece por encima o por debajo del subtítulo del punto de la historia una vez que arrastre su primer punto de la historia en el lienzo y pase el ratón sobre el área del navegador. Úsela para revertir cambios, aplicar las actualizaciones pertinentes a un punto de la historia, eliminar un punto de la historia o crear uno a partir del punto de la historia personalizado actual. Todas las opciones están disponibles una vez que realice un cambio en el punto de la historia. De lo contrario, solo está disponible la opción de supresión.

#### Compruebe su trabajo. Vea "Crear el primer punto de la historia" y "Destacar las ventas de máquinas" en acción.

<img src="../images/04/13.gif" width="800" >

#### Argumentar su idea

La conclusión es que las máquinas de Carolina del Norte pierden dinero para tu empresa. Ha descubierto esto en el dashboard que ha creado. Solo con ver las ventas generales y las ganancias por año no se puede demostrar este argumento, pero las ganancias regionales sí que pueden.

1. En el panel `Historia`, seleccione En blanco. Después, arrastre el dashboard Regional `Sales` and `Profit` (Ventas y ganancias regionales) al lienzo.

Esto ofrece a los asistentes una nueva perspectiva de sus datos: las ganancias negativas captan su atención.

<img src="../images/04/14.png" width="600" >

2. Agrega un subtítulo, como "Underperforming items in the South".

Para restringir los resultados solo a North Carolina, empiece con un punto de la historia duplicado.

- Selecciona Duplicar para crear otro punto de la historia con el dashboard Regional Profits.
- Selecciona North Carolina en el mapa y observe que el gráfico de barras se actualiza automáticamente.
- Selecciona Todo en la tarjeta de filtro Año de fecha de pedido.
- Añada un subtítulo, por ejemplo "`Profit` in North Carolina, 2018-2021" (beneficios en Carolina del Norte 2018-2021).

Ahora puede mostrar a los asistentes los cambios en las ganancias producidos al año en North Carolina. Para hacerlo, creará cuatro puntos de la historia:

- Selecciona Duplicar para empezar con el dashboard Regional `Profit` centrado en North Carolina.
- En el filtro Año de fecha de pedido, haga clic en el botón de flecha derecha para que aparezca 2018.
- Añada un subtítulo, por ejemplo "`Profit` in North Carolina, 2018", y haga clic en Duplicar.
- Repite los pasos 2 y 3 para los años 2019, 2020 y 2021.

Ahora los asistentes se harán una idea de qué productos se introdujeron en el mercado de North Carolina y cuál fue su rentabilidad en el tiempo.

#### Compruebe su trabajo. Vea "Argumentar su idea" en acción.

<img src="../images/04/15.gif" width="800" >

#### Retoques finales

En este punto de la historia, que está centrado en los datos de 2021, describa tus hallazgos. Agregamos más detalles que solo un título.

1. En el panel de la izquierda, seleccione Arrastrar para añadir texto y arrástrelo a la vista.

2. Introduce una descripción para el dashboard donde se enfatice el mal rendimiento de las máquinas de North Carolina, por ejemplo, "La presentación de las máquinas en el mercado de Carolina del Norte en 2021 ha provocado pérdidas de una cantidad significativa de dinero".

Para un efecto dramático, puede situar el cursor sobre ``Machines`` en el gráfico de barras ``Sales` in the South` (Ventas en el sur) durante la presentación, para mostrar una descripción emergente útil: la pérdida de casi 4000 dólares estadounidenses.

<img src="../images/04/16.png" width="800" >

Y, ahora, para la última diapositiva, profundice en los detalles.

3. En el panel `Historia`, haga clic en En blanco.

4. En el panel `Historia`, arrastre Gráfico de barras de ganancias negativas a la vista.

5. En la tarjeta de filtro Año de fecha de pedido, filtre la vista solo hasta 2021.

Ahora verá fácilmente que la pérdida de ganancias por máquinas procedía exclusivamente de Burlington, Carolina del Norte.

6. En la vista, haga clic con el botón derecho en la marca Burlington (la barra) y seleccione Anotar > Marca.

7. En el cuadro de diálogo Editar anotación que aparece, elimine el texto de relleno y escriba: "Las máquinas de Burlington supusieron unas pérdidas de casi 4000 dólares estadounidenses en 2021".
Haz clic en Aceptar.

8. En la vista, haga clic en la anotación y arrástrela para ajustarla donde aparezca.

9. Asigne a este punto de la historia el subtítulo: "¿Dónde estamos perdiendo ganancias de máquinas en Carolina del Norte?"

10. Haga doble clic en la pestaña `Historia` 1 y cambie el nombre a la historia, como "Mejorar las ganancias en el sur".

11. Revise la historia (seleccione Ventana > Modo de presentación).

#### Ajuste al tamaño

¿Qué son las barras de desplazamiento que aparecen en la parte derecha o en la parte inferior del punto de la historia del dashboard mientras está en el modo de presentación?

<img src="../images/04/17.png" width="800" >

Parece que el dashboard es demasiado grande para la presentación. Qué fastidio. Presione la tecla Esc para salir de la presentación y, a continuación, seleccione la hoja `Ganancias` regionales en la parte inferior del libro de trabajo.

En el panel izquierdo, debajo de ``Dashboard``, cambie la selección de la lista desplegable Tamaño de Escritorio a Ajustar para Mejorar las ganancias en el sur. De esta forma, se cambiará automáticamente el tamaño del dashboard para visualizar la historia de forma óptima.

<img src="../images/04/18.png" width="400" >

Selecciona Ajustar para mejorar las ganancias en el sur y después vuelva a activa el modo de presentación. Se ajustará correctamente el tamaño del dashboard.

#### Compruebe su trabajo. Vea "Retoques finales" en acción.

<img src="../images/04/19.gif" width="800" >
