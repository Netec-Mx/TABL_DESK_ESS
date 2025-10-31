# Análisis Avanzado

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
1.	xxxxxxx


## Objetivo Visual 

<img src="../images/05/00.png" width="500" >



## Duración aproximada:
- 90 minutos.


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

- Pestaña de Análisis: herramienta para explorar patrones, tendencias y detalles en datos.
- Arrastrar y soltar objetos analíticos: líneas, bandas, áreas, totales → destacan aspectos clave.
- Líneas de referencia: promedios, medianas, mínimos o máximos → contextualizan datos.
- Barras de referencia: marcan rangos o límites específicos en la visualización.
- Líneas de tendencia: muestran comportamiento en el tiempo o frente a otra variable (lineal, exponencial, logarítmico).
- Previsiones: proyectan tendencias futuras con base en datos históricos.
- Cálculos rápidos de tabla: porcentajes, diferencias, totales → aplicados desde pestaña Análisis.
- Resaltado: reglas para identificar valores atípicos o áreas de interés.
- Agrupación y clústeres: grupos automáticos según similitudes en los datos.

--DIAPOSITIVA 42.

<img src="../images/05/16.jpg"  >
<img src="../images/05/17.jpg"  >
<img src="../images/05/18.jpg"  >
<img src="../images/05/19.jpg"  >
<img src="../images/05/20.jpg"  >
<img src="../images/05/21.jpg"  >
<img src="../images/05/22.jpg"  >
<img src="../images/05/23.jpg"  >
<img src="../images/05/24.jpg"  >
<img src="../images/05/25.jpg"  >
<img src="../images/05/26.jpg"  >
<img src="../images/05/27.jpg"  >
<img src="../images/05/28.jpg"  >
<img src="../images/05/29.jpg"  >
<img src="../images/05/30.jpg"  >
<img src="../images/05/31.jpg"  >
<img src="../images/05/32.jpg"  >
<img src="../images/05/33.jpg"  >
<img src="../images/05/34.jpg"  >
<img src="../images/05/35.jpg"  >
<img src="../images/05/36.jpg"  >
<img src="../images/05/37.jpg"  >
<img src="../images/05/38.jpg"  >
<img src="../images/05/39.jpg"  >
<img src="../images/05/40.jpg"  >
<img src="../images/05/41.jpg"  >
<img src="../images/05/42.jpg"  >
<img src="../images/05/43.jpg"  >
<img src="../images/05/44.jpg"  >
<img src="../images/05/45.jpg"  >
<img src="../images/05/46.jpg"  >
<img src="../images/05/47.jpg"  >
<img src="../images/05/48.jpg"  >
<img src="../images/05/49.jpg"  >
<img src="../images/05/50.jpg"  >
<img src="../images/05/51.jpg"  >
<img src="../images/05/52.jpg"  >
<img src="../images/05/53.jpg"  >
<img src="../images/05/54.jpg"  >
<img src="../images/05/55.jpg"  >
<img src="../images/05/56.jpg"  >
<img src="../images/05/57.jpg"  >
<img src="../images/05/58.jpg"  >
<img src="../images/05/59.jpg"  >
<img src="../images/05/60.jpg"  >
<img src="../images/05/61.jpg"  >
<img src="../images/05/62.jpg"  >
<img src="../images/05/63.jpg"  >
<img src="../images/05/64.jpg"  >
<img src="../images/05/65.jpg"  >
<img src="../images/05/66.jpg"  >
<img src="../images/05/67.jpg"  >
<img src="../images/05/68.jpg"  >
<img src="../images/05/69.jpg"  >
<img src="../images/05/70.jpg"  >
<img src="../images/05/71.jpg"  >
<img src="../images/05/72.jpg"  >
<img src="../images/05/73.jpg"  >
<img src="../images/05/74.jpg"  >
<img src="../images/05/75.jpg"  >
<img src="../images/05/76.jpg"  >
<img src="../images/05/77.jpg"  >
<img src="../images/05/78.jpg"  >
<img src="../images/05/79.jpg"  >
<img src="../images/05/80.jpg"  >
<img src="../images/05/81.jpg"  >
<img src="../images/05/82.jpg"  >
<img src="../images/05/83.jpg"  >
<img src="../images/05/84.jpg"  >
<img src="../images/05/85.jpg"  >
<img src="../images/05/86.jpg"  >
<img src="../images/05/87.jpg"  >
<img src="../images/05/88.jpg"  >
<img src="../images/05/89.jpg"  >
<img src="../images/05/90.jpg"  >
<img src="../images/05/91.jpg"  >
<img src="../images/05/92.jpg"  >
<img src="../images/05/93.jpg"  >
<img src="../images/05/94.jpg"  >
<img src="../images/05/95.jpg"  >
<img src="../images/05/96.jpg"  >
<img src="../images/05/97.jpg"  >
<img src="../images/05/98.jpg"  >
<img src="../images/05/99.jpg"  >
<img src="../images/05/100.jpg"  >
<img width="161" height="3421" alt="image" src="https://github.com/user-attachments/assets/dae3e1de-1831-43d6-b5ed-3c7dab8d977e" />
