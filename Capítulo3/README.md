# Práctica 3. Análisis y filtros en Tableau 

## Objetivos
Al finalizar la práctica, serás capaz de:
- Centrarte en los `Datos` relevantes mediante filtros y colores para analizar con mayor precisión los resultados en Tableau Desktop.
- Analizar las tendencias geográficas de ventas y rentabilidad creando una vista de mapa en Tableau para visualizar patrones por región.
- Profundizar en el análisis filtrando los `Datos` para centrarse en los estados con pérdidas y descubrir las causas de las ganancias negativas.


## Objetivo visual 

<img src="../images/03/00.png" width="500" >



## Duración aproximada
- 90 minutos.


## Instrucciones 

### Tarea 1. Centrarse en los resultados

Has creado una vista de ventas de productos, organizada por categoría y `Sub-Category`. Aunque ya tienes un avance, la cantidad de `Datos` hace que sea difícil ordenarlos. Necesitas identificar rápidamente los puntos más relevantes y enfocarte en resultados concretos. Afortunadamente, Tableau ofrece excelentes opciones para lograrlo.

Mediante el uso de filtros y colores, puedes centrarte más en los detalles que te interesan. Después de centrarse en ciertos `Datos`, puedes empezar a utilizar otras características de Tableau Desktop para interactuar con esos `Datos`.

#### Añadir filtros a la vista

Puedes utilizar filtros para incluir o excluir valores en la vista. En este ejemplo, agrega dos filtros sencillos a la hoja de trabajo para que sea más sencillo ver las ventas de productos por subcategoría para un determinado año.

1. En el panel `Datos`, haz clic con el botón derecho en `Order Date` y selecciona `Mostrar filtro`.

2. Repite el paso anterior para el campo `Sub-Category`.

Los filtros se añaden al lateral derecho de la vista en el orden en que los seleccionaste. Los filtros son tipos de tarjeta y se pueden mover por el lienzo haciendo clic en el filtro y arrastrándolos a otro sitio de la vista. A medida que arrastres el filtro, aparecerá una línea que muestra dónde puedes colocar el filtro para moverlo.

> **Nota**
> 
> Para el tutorial, utiliza la posición predeterminada de las tarjetas de filtro.

<img src="../images/03/01.png" width="350" >


#### Comprueba tu trabajo. Observa `Aplicar filtros a la vista` en acción

<img src="../images/03/02.gif" width="800" >


#### Agregar color a la vista

Al agregar filtros es más fácil ordenar todos estos `Datos` pero, ¡se ve mucho el color azul! Es hora de que lo .

Lo que observas ahora son los totales de ventas para los distintos productos. Puedes ver que algunos productos tienen ventas consistentemente bajas y algunos productos pueden ser buenos candidatos para reducir los esfuerzos de ventas para esas líneas de productos. Pero, ¿cómo se ve la rentabilidad general de sus productos? arrastres `Profit` a `Color` para saber qué ocurre.

En el panel `Datos`, arrastra `Profit` hasta `Color` en la tarjeta `Marcas`.

Al arrastrar `Profit` a `Color`, puedes ver que tienes ganancias negativas en `Tables`, `Bookcases` e incluso `Machines`. ¡Has descubierto otro dato útil!

<img src="../images/03/03.png" width="800" >

> **Nota**
> 
> Tableau ha añadido automáticamente una leyenda de color y ha asignado una paleta de colores divergentes, porque los `Datos` incluyen valores negativos y positivos.


#### Trabajar con colores

Al agregar colores, mejora el aspecto de la vista, pero también puedes ayudar a revelar datos interesantes. Tableau utiliza una paleta de colores predeterminada para asignar colores a los productos de la vista, pero no está limitado a utilizar esa paleta de colores. ¡Hay más opciones!

Si deseas utilizar colores distintos de los que se muestran, puedes cambiar los colores o la paleta de colores cuando quieras. Solo tienes que hacer clic en `Color`en la tarjeta `Marcas` y, después, en `Editar colores`. Puedes seleccionar otra paleta de colores distinta en el cuadro de diálogo abierto de `Editar colores`.

> **Nota**
>
> Para el tutorial se utiliza la paleta de colores predeterminada.

En función de los `Datos` de la vista, es posible que el cuadro de `Editar colores` muestre una paleta de colores divergentes en lugar de una paleta de colores categórica.

Las paletas de colores divergentes tienen el aspecto de la imagen siguiente y suelen asignarse a campos continuos.

<img src="../images/03/04.png" width="350" >

Si utilizas una leyenda, puede que tenga el aspecto de la imagen de abajo. Las paletas de colores categóricas como esta suelen asignarse a campos discretos.

<img src="../images/03/05.png" width="400" >

#### Comprueba el trabajo. Observa "Agregar color a la vista" en acción

<img src="../images/03/06.gif" width="800" >

#### Encontrar información útil esencial

Como ya hemos dicho, puedes explorar los datos a medida que creas vistas con Tableau Desktop. Al agregar filtros y colores, es más fácil visualizar los datos e identificar los problemas al instante.

La siguiente parada consiste en interactuar con la vista para empezar a extraer conclusiones.

Al examinar la vista, notaste que algunos productos no son rentables en absoluto; ahora, comprueba si estos productos han sido poco rentables a lo largo de los años.

Es el momento de utilizar los filtros para examinarlos más de cerca.

1. En la vista, en la tarjeta de filtro `Sub-Category`, desactiva todas las casillas de verificación excepto `Bookcases`, `Machines` y `Tables`.

<img src="../images/03/07.png" width="700" >

Ahora puedes ver que, en algunos años, `Bookcases` y `Machines` fueron realmente rentables. Sin embargo, recientemente, `Machines` ha dejado de ser rentable. Aunque has descubierto algo importante, recopila la información antes de proponer cualquier elemento de acción a tu jefa.

Al desglosar la vista por regiones:

2. Selecciona `Todo` en el filtro `Sub-Category` para mostrar todas las categorías de nuevo.

3. Desde el panel `Datos`, arrastra `Region` al estante `Filas` y colócalo a la derecha de `Sum(Sales)`.

Tableau crea una vista con varios ejes desglosados por región.

<img src="../images/03/08.png" width="700" >

Ahora puedes ver las ventas y la rentabilidad por producto para cada región. Al agregar la región a la vista y filtrar la subcategoría para que muestre solo `Machines`, observas que indican unas ganancias negativas en el sur más elevadas que en otras regiones de manera general. ¡Has descubierto un dato útil que estaba oculto!

<img src="../images/03/09.png" width="700" >

Esta vista es la que mejor resume el trabajo hasta ahora. Selecciona `Todo` en la tarjeta de filtro `Sub-Category` (si cambiaste el filtro) para mostrar todas las subcategorías de nuevo y, a continuación, ponle nombre a la hoja de trabajo y añade un título.

4. En la parte inferior izquierda del espacio de trabajo, haz doble clic en `Hoja 1` y escribe `Ventas` por producto/región.

Centra el análisis en `South`, pero no pierdas la vista que has creado. En Tableau Desktop, puedes duplicar la hoja de trabajo para seguir trabajando donde lo dejaste.

5. En el libro de trabajo, haz clic con el botón derecho en la hoja `Ventas` por producto/región y selecciona `Duplicar` .

6. Cambia el nombre de la hoja duplicada a `Sales in the South`.

7. En la nueva hoja de trabajo, desde el panel `Datos`, arrastra `Region` al estante `Filtros` para agregarlo como un filtro en la vista.

8. En el cuadro de diálogo del filtro `Region`, desactiva todas las casillas de verificación excepto `South` y haz clic en `Aceptar`.

La vista se actualiza para tener el aspecto de la siguiente imagen.

<img src="../images/03/10.png" width="700" >

Ahora puedes centrarte en las ventas y las ganancias en `South`. Inmediatamente, notas que las ventas de `Machines` tienen ganancias negativas en 2018 y de nuevo en 2021. ¡Está claro que tienes que investigar este dato!

1. Guarda el trabajo seleccionado `Archivo > Guardar como`. Asigna un nombre al libro de trabajo, como `Regional Sales and Profits`.

#### Cómo organiza Tableau los libros de trabajo guardados

Cuando instala Tableau, se crea automáticamente un directorio de carpetas en `Documentos > Mis documentos > Mi repositorio de Tableau`; la cual contiene varias carpetas para fuentes de `Datos`, libros de trabajo guardados, datos de geocodificación y mucho más.

#### Comprueba el trabajo. Observa `Encontrar información útil esencial` en acción

<img src="../images/03/11.gif" width="800" >

#### Resumen de los pasos

En esta tarea, has aprendido a:
- Aplicar filtros y colores para concentrarte más fácilmente en aquellas áreas de datos relevantes.
- Interactuar con el gráfico utilizando las herramientas que proporciona Tableau.
- Duplicar hojas de trabajo y guardar los cambios para seguir explorando los datos de distintos modos sin perder el trabajo.

Tras explorar los datos en Tableau Desktop, has detectado algunas áreas que merecen atención. Ahora sabes que las ventas y las ganancias en la región sur son un problema, pero aún no has encontrado una solución. Analiza otros factores que pueden contribuir a obtener estos resultados. A continuación, aprovecha otra característica esencial de Tableau para trabajar con datos geográficos.



### Tarea 2. Explorar los datos geográficamente

Has creado una vista muy práctica que permite revisar las ventas y las ganancias producto a producto a lo largo de varios años. Después de fijarte en las ventas de productos y en la rentabilidad de la zona `South`, busca tendencias o patrones en esa región.

Como estás buscando datos geográficos (el campo `Region`), tienes la opción de crear una vista de mapa. Las vistas de mapa son ideales para mostrar y analizar este tipo de información.

Para este ejemplo, Tableau ya ha asignado funciones geográficas adecuadas a los campos `Country`, `State`, `City` y `Postal Code`. El motivo es que reconoció que cada uno de estos campos contenía datos geográficos. Puedes crear directamente la vista de mapa.

#### Conocer las funciones geográficas

Tableau reconoce una gran variedad de datos geográficos comunes (por ejemplo, nombres de estados y ciudades). Cuando Tableau los reconoce, asigna de forma automática las funciones adecuadas a los campos, para que se conviertan en campos geográficos.

En el panel `Datos`, los campos geográficos tienen iconos de globo que identifica campos de datos geográficos al lado. Si se asigna una función geográfica a un campo, Tableau crea automáticamente una vista de mapa al agregar el campo a `Detalle` en la tarjeta `Marcas`. Más adelante se abordará más sobre esto.

Si Tableau no reconoce los datos como geográficos, puedes asignar manualmente una función geográfica a cada uno de los campos relevantes.

Hay varias funciones geográficas entre las que elegir:

- Aeropuerto
- Código de área
- CBSA/MSA
- Ciudad
- Distrito electoral
- País/región
- Provincia/Municipio/Condado
- NUTS Europa
- CC. AA./Estado/Provincia/Dpto.
- Código postal

Para verlo en acción, consulta la siguiente animación.

<img src="../images/03/12.gif" width="600" >


#### Crear una vista de mapa

Empieza de cero con una nueva hoja de trabajo.

1. Al final del libro de trabajo, haz clic en el icono `Nueva hoja de trabajo`.

<img src="../images/03/13.png" width="600" >

Tableau conserva la hoja anterior y crea una nueva para que puedas continuar explorando los `Datos` sin perder el trabajo.

2. En el panel `Datos`, haz doble clic en `State` para agregarlo a`Detalle` en la tarjeta `Marcas`.

Ya tienes una vista de mapa.

<img src="../images/03/14.png">


#### Hacer doble clic para agregar campos geográficos

Puedes hacer doble clic en los campos para agregarlos rápidamente a la vista. Cuando hace doble clic en un campo geográfico, se agrega automáticamente a `Detalles` en la tarjeta `Marcas` y se crea una vista de mapa con marcas para cada ubicación enumerada en el campo.

Como Tableau ya sabe que los nombres de estado son datos geográficos y la dimensión `State` está asignada a la función geográfica CC. AA./Estado/Provincia/Dpto., Tableau crea automáticamente una vista de mapa.

Ten en cuenta que el campo `Country` también se agrega a la vista. Esto ocurre porque los campos geográficos en `Muestra - Supertienda` forman parte de una jerarquía. Cada nivel de la jerarquía se agrega como un nivel de detalle.

Además, los campos Latitud y Longitud se agregan a los estantes `Columnas` y `Filas`. Puedes considerarlos como campos X e Y. Son esenciales para cuando quiera crear una vista de mapa, porque cada ubicación de los `Datos` se asigna a un valor de latitud y de longitud. A veces, los campos Latitud y Longitud los genera Tableau. Otras veces, es posible que quiera incluirlos manualmente en los `Datos`. En la Biblioteca de aprendizaje encontrará recursos para profundizar más en este tema.

Bien, una cosa es tener un interesante mapa que se centra en los 48 estados pero, ¿se acuerda de que lo que quería era saber qué ocurría en la región South?

3. arrastres `Region` al estante `Filtros`  y, después, filtre solo por South. La vista de mapa amplía la región South, donde hay una marca para cada estado (11 en total).

Ahoragustaría ver `Datos` más detallados para esta región, así que empieza a arrastrar otros campos a la tarjeta `Marcas`:

4. arrastres la medida `Sales` a `Color`en la tarjeta `Marcas`.

<img src="../images/03/15.gif" width="800" >

La vista se actualiza automáticamente a un mapa rellenado, donde cada estado está representado por un color según el total de ventas. Debido a que está explorando las ventas de productos, deseas que sus ventas aparezcan en USD. Haz clic en el campo Sum(`Sales`) en el estante `Columnas` y selecciona Formato. En Números, selecciona Moneda.

Cada vez que añade una medida continua que contiene número positivos (por ejemplo, `Ventas` ) a `Color`en la tarjeta `Marcas`, el mapa rellenado con `Datos` se vuelve azul. A los valores negativos se les asigna el naranja.

Puedes que en ocasiones no quiera que el mapa sea azul. Quizá prefiera el verde o piense que ciertos `Datos` no se deben representar de color azul, como en el caso de incendios forestales o atascos. Resultaría muy confuso.

No hay problema, puedes cambiar la paleta de colores como hizo antes.

5. Haz clic en `Color`en la tarjeta `Marcas` y selecciona `Editar colores`.

Para este ejemplo, deseas saber qué estados tienen buenos resultados en ventas y cuáles no.

6. En la lista desplegable Paleta, selecciona Rojo-verde divergente y haz clic en Aceptar. Estopermite ver rápidamente los estados que tienen peores resultados y los que tienen mejores resultados.

La vista se actualiza y tienes más o menos este aspecto:

<img src="../images/03/16.png" width="400" >

Espere un momento: ¡Todo se ha puesto en rojo! ¿Qué ha ocurrido?

Los `Datos` son correctos y, técnicamente, puedes comparar los estados con peores resultados con respecto a los que tienen buenos resultados. ¿Pero hay algo más que no sabe?

¿Realmente las ventas en estos estados son tan terribles o simplemente hay más personas en Florida que quieren comprar sus productos? Quizá en los estados que se muestran en rojo hayas menos tiendas o estas sean más pequeñas. O quizá hayas una mayor densidad de población en los estados que se muestran en verde, así que hay más gente para comprar los productos.

En cualquier caso, no quiere mostrar esta vista tal cual a el jefa porque no está convencido de que los `Datos` estén transmitiendo información útil.

7. Haz clic en el icono Deshacer <img src="../images/03/17.png" > de la barra de herramientas para volver a la vista azul que tantogustaba.

igue habiendo un problema con el color. Así todo parece perfecto, ¡ese es el problema!

A primera vista, parece que Florida es el estado con mejores resultados. Al situar el cursor sobre el marca, descubre que tienes un total de ventas de 89 474 dólares estadounidenses, comparado por ejemplo con South Carolina, cuyas ventas solo son 8482 dólares estadounidenses. Sin embargo, ¿ha resultado rentable alguno de la región South?

8. arrastres Ganancias a `Color`en la tarjeta `Marcas` para ver si encuentra una respuesta a esta pregunta.

<img src="../images/03/18.png" width="400" >

¡Así mejor! Puesto que a menudo las ganancias están formadas por valores positivos y negativos, Tableau selecciona automáticamente la paleta de colores divergentes Naranja-Azul para mostrar rápidamente los estados con ganancias negativas y con ganancias positivas.

Ahora se ve claramente que Tennessee, North Carolina y Florida tienen ganancias negativas, aunque pareciera que daban buenos resultados (incluso excelentes) en `Sales`. ¿Pero por qué? Encontrará la respuesta en el paso siguiente

#### Comprueba el trabajo. Observa "Crear una vista de mapa" en acción

<img src="../images/03/19.gif" width="800" >


### Tarea 3. Desglosar los detalles

En el último paso, descubrió que Tennessee, North Carolina y Florida tienen ganancias negativas. Para averiguar por qué, decide profundizar aún más y centrarse en qué ocurre solo en estos tres estados.

#### Retomar por donde se quedó con la vista de mapa

Como vimos en el último paso, los mapas son estupendos para visualizar los `Datos` de manera general. El gráfico de barrasayudará a ir al grano. Para hacerlo, cree otra hoja de trabajo.

1. Haz doble clic en Hoja 3 y asígnele el nombre `Profit` Map.

2. Haz doble clic en `Profit` Map al final del área de trabajo y selecciona `Duplicar` . Asigne el nombre Negative `Profit` Bar Chart a la nueva hoja.

3. En la hoja de trabajo Negative `Profit` Bar Chart, haz clic en Mostrarme y selecciona barras horizontales.

Mostrarme destaca tipos de gráficos distintos según los `Datos` que ha agregado a la vista.

> **Nota**
> Cuando lo desee, puedes volver a hacer clic en Mostrarme para contraerlo.

<img src="../images/03/20.png" width="350" >

Ya vuelve a tener un gráfico de barras, así de fácil.

<img src="../images/03/21.png" width="700" >

4. Para seleccionar varias barras en la izquierda, selecciona y arrastres el cursor por varias de las barras situadas entre Tennessee, North Carolina y Florida para seleccionar las barras de la izquierda. En la descripción emergente que aparece, selecciona Mantener solamente para centrarse en estos tres estados.

> **Nota**
> también puedes hacer clic con el botón derecho en las barras destacadas y seleccionar Mantener solamente.

Tenga en cuenta que el campo Inclusiones para `State` se agrega al estante `Filtros`  para indicar que ciertos estados están filtrados en la vista. El icono con dos círculos en el campo indica que este campo es un conjunto. Puedes editarlo haciendo clic con el botón derecho en el campo en el estante `Filtros`  y seleccionando Editar filtro.

Ahora quiere ver los `Datos` de las ciudades en estos estados.

5. En el estante `Filas`, haz clic en el icono de suma en el campo `State` para desglosar al nivel de detalle `City`.

Aquí hay demasiada información, así que decide filtrar la vista a las ciudades con las ganancias más negativas usando un filtro Top N.


#### Comprueba el trabajo. Observa los pasos del 1 al 5 en acción

<img src="../images/03/22.gif" width="800" >

#### Crear un filtro N superior

Puedes utilizar un filtro N superior en Tableau Desktop para establecer un límite para el número de marcas que se muestran en la vista. En este caso, deseas utilizar el filtro N superior para centrarse en los que tienen menos ganancias.

1. En el panel `Datos`, arrastres `City` al estante `Filtros` .

2. En el cuadro de diálogo Filtro, selecciona la pestaña Superior y haz lo siguiente:

- Haz clic en *Por campo*.
- Haz clic en la lista desplegable *Superior* y selecciona *Inferior* para mostrar los que obtuvieron menos ganancias.
- Escriba *5* en el cuadro de texto para mostrar los 5 con peores resultados en el conjunto de `Datos`.

Tableau Desktop ya ha seleccionado un campo (`Profit`) y agregación (Suma) para el filtro N superior según los campos de la vista. Esta configuración garantiza que la vista mostrará solo las cinco ciudades con peor rendimiento por suma de ganancias.

<img src="../images/03/23.png" width="500" >

- Haz clic en Aceptar.

¿Qué pasó con el gráfico de barras y por qué está en blanco? Se trata de una buena pregunta y de una buena oportunidad para presentar el orden de las operaciones en Tableau.

El orden de las operaciones en Tableau, también conocido como proceso de consulta, es el orden en que Tableau realiza las distintas acciones, como el orden en que aplica los filtros del usuario a la vista.

Tableau aplica los filtros en el siguiente orden:

- `Filtros`  de extracciones
- `Filtros`  de fuentes de `Datos`
- `Filtros`  de contexto
- `Filtros`  de N primeros
- `Filtros`  de dimensión
- `Filtros`  de medidas

El orden en el que cree los filtros o en el que los organice en el estante `Filtros`  no modifica el orden en el que Tableau los aplica en el vista.

Lo bueno es que puedes indicarle a Tableau que cambie este orden cuando detecte que algo extraño está sucediendo a los filtros de la vista. En este ejemplo, el filtro Top N se aplica a las cinco ciudades con peor rendimiento por suma de ganancias para todo el mapa, pero ninguna de esas ciudades está en el sur, por lo que el gráfico está en blanco.

Para arreglar el gráfico, agregue un filtro al contexto. Esto indicará a Tableau que filtre primero ese campo, con independencia de si se ajusta al orden de operaciones.

Pero, ¿qué campo agrega al contexto? Hay tres campos en el estante `Filtros` : Región (filtro de dimensión), Ciudad (filtro de N primeros) e Inclusiones (País, Estado) (País, Estado) (conjunto).

Si vuelve a observar el orden de operaciones, sabrá que el conjunto y el filtro de N primeros se están aplicando antes que el filtro de dimensión. ¿Pero sabe si el filtro de los N primeros o el filtro de conjunto se ha aplicado primero? Vamos a verlo.

3. En el estante `Filtros` , haz clic con el botón derecho en el campo Ciudad y selecciona Agregar a contexto.

El campo Ciudad se atenúa y pasa a la parte superior del estante `Filtros` , pero en la vista no cambia nada. Por lo que, incluso aunque esté forzando a Tableau a filtrar primero por Ciudad, el problema no se resuelve.

4. Haz clic en Deshacer.

5. En el estante `Filtros` , haz clic con el botón derecho en el conjunto Inclusiones (País, Estado) (País, Estado) y selecciona Agregar a contexto

El conjunto Inclusiones (País, Estado) (País, Estado) se atenúa y pasa al principio del estante `Filtros` . ¡Y las barras vuelven a la vista!

Va por buen camino. Pero hay seis ciudades, incluida Jacksonville y Carolina del Norte, que tienen una ganancia positiva. ¿Por qué aparece en la vista una ciudad con ganancias positivas si ha creado un filtro que se supone que debía eliminarla de la vista?

Jacksonville (Carolina del Norte) se ha incluido porque Ciudad es el nivel de detalle mínimo que se muestra en la vista. Para que Tableau Desktop conozca la diferencia entre Jacksonville (Carolina del Norte) y Jacksonville (Florida), necesita profundizar al siguiente nivel de detalle en la jerarquía de ubicación que, en este caso, es `Postal Code`. Después de añadir este nivel de detalle, puedes excluir Jacksonville de North Carolina sin tener que excluir Jacksonville de Florida.

6. En el estante `Filas`, haz clic en el icono de suma en `City` para profundizar al nivel de detalle `Postal Code`.

7. Haz clic con el botón derecho en el código postal para Jacksonville (Carolina del Norte) 28540 y selecciona Excluir.

`Postal Code` se agrega al estante `Filtros`  para indicar que algunos miembros del campo `Postal Code` se han filtrado de la vista. Aunque se elimine el campo `Postal Code` de la vista, el filtro permanecerá.

8. arrastres `Postal Code` fuera del estante `Filas`.

La vista se actualiza y tienes más o menos este aspecto:

<img src="../images/03/24.png" width="700" >

#### Comprueba el trabajo. Observa los pasos del 1 al 8 en acción

<img src="../images/03/25.gif" width="800" >

#### Identificar los menos rentables

Decides desglosar la vista por `Sub-Category` para identificar los productos que están mermando las ganancias. Como sabe que el campo `Sub-Category` contiene información sobre los productos vendidos por ubicación, decide comenzar ahí.

1. arrastres `Sub-Category` al estante `Filas` y colócalo a la derecha de `City`.

2. arrastres `Profit` a `Color`en la tarjeta `Marcas` para que resulte más fácil ver qué productos tienen ganancias negativas.

3. En el panel `Datos`, haz clic con el botón derecho en `Order Date` y selecciona `Mostrar filtro`.

Ahora, si lo desea, puedes explorar los beneficios negativos para cada año y detectar rápidamente los productos que están perdiendo dinero.

Parece que `Machines`, `Tables` y Binders no están dando buenos resultados. Así que, ¿qué tal si deja de vender esos artículos en Jacksonville, Concord, Burlington, Knoxville y Memphis?

<img src="../images/03/26.png" width="800" >

#### Comprobar los hallazgos

Si se elimina Binders, `Machines` y `Tables`, ¿mejorarán las ganancias en Florida, North Carolina y Tennessee? Para averiguarlo, puedes filtrar los productos que dan problemas para ver qué ocurre.

1. Vuelva a la vista de mapa haciendo clic en la pestaña de la hoja `Profit` Map.

2. En el panel `Datos`, haz clic con el botón derecho en `Sub-Category` y selecciona `Mostrar filtro`.

Junto a la vista de mapa se muestra una tarjeta de filtro para todos los productos que ofrece. Utilizará este filtro más tarde.

3. En el panel `Datos`, arrastres `Profit` y `Profit` Ratio a Etiqueta en la tarjeta `Marcas`. Para dar formato a la Relación de beneficios como porcentaje, haz clic con el botón derecho en Relación de beneficios y selecciona Formato. Luego, para Números predeterminados, elija Porcentaje y establezca el número de lugares decimales que deseas que se muestren en el mapa. Para este mapa, elegiremos cero lugares decimales.

Ahora puedes ver las ganancias exactas de cada estado sin tener que situar el cursor sobre ellos.

4. En el panel `Datos`, haz clic con el botón derecho en `Order Date` y selecciona `Mostrar filtro` para proporcionar algo de contexto a la vista.

Se muestra una tarjeta de filtro para YEAR(`Order Date`) en la vista. Ya puedes ver las ganancias de todos los años o de una combinación de años. Esto puedes resultar útil para la presentación.

5. Borre Binders, `Machines` y `Tables` de la lista en la tarjeta de filtro `Sub-Category` en la vista.

No olvide que al agregar filtros a la vista, podrá incluir y excluir valores para destacar ciertos elementos de los `Datos`.

Después de eliminar cada miembro, mejoran las ganancias para Tennessee, North Carolina y Florida hasta que, finalmente, cada estado tienes ganancias positivas.

<img src="../images/03/27.gif" width="800" >

Este descubrimiento es muy interesante.

Binders, `Machines` y `Tables` son definitivamente los responsables de las pérdidas en Tennessee, North Carolina y Florida, pero no en el resto de la región South. ¿Has notado cómo las ganancias disminuyen en realidad para otros estados cuando borra artículos de la tarjeta de filtro? Si, por ejemplo, conmuta Binders (Carpetas) en la tarjeta de filtro Subcategoría, las ganancias caen un cuatro por ciento en Arkansas. Puedes deducir que las carpetas son rentables en Arkansas.

Quieres compartir este hallazgo con el equipo y para ello quiere que sigan los mismos pasos hechos por tú.

6. Selecciona (Todos) en la tarjeta de filtro `Sub-Category` para incluir todos los productos de nuevo.

Has averiguado que Binders, `Machines` y `Tables` son los responsables de las ganancias negativas en Tennessee, North Carolina y Florida. ¿Y ahora qué?

Puedes seguir explorando los `Datos` respondiendo a las preguntas de abajo. > **Nota** > > Si usa la vista para explorar estas preguntas, deshaz cualquier cambio antes de continuar con el tutorial Introducción.

- ¿Cómo son las ventas de `Machines` en Tennessee, North Carolina y Florida? ¿Se está vendiendo mucho? En ese caso, ¿cómo afectan a las ganancias?
- ¿Qué otros factores pueden estar contribuyendo a estos resultados? ¿Los minoristas de la región South están vendiendo productos con descuento?
- ¿Qué ocurre con las ventas de `Tables` y Binders?
- ¿Qué ocurre con las ventas en Jacksonville, Miami, Burlington, Knoxville y Memphis cuando quitamos `Machines`, `Tables` o Binders?
- ¿Y qué ocurre con `Bookcases`? Recuerde que en el paso 2 vimos que `Bookcases` no era nada rentable en otras regiones. Si profundiza en esas regiones, podrá descubrir otras soluciones.

#### Comprueba el trabajo. Observa "Comprobar los hallazgos" en acción

<img src="../images/03/28.gif" width="900" >

Ya sabe que `Machines`, `Tables` y Binders son productos problemáticos para el empresa. Al centrarse en el sur, comprueba que estos productos tienen un impacto variable en las ganancias. Puedes que merezca la pena comentar esto con el jefa.

A continuación, recopilará el trabajo que ha realizado hasta ahora en un dashboard para poder presentar sus hallazgos de manera clara.
