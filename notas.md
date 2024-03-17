# 1 El documento Html

Todos los docuemtos Html se componen de unos elementos principales:

**La cabeza o head**  < head > < /head > 

Aquí va todo lo relacionado con los metadatos de la página, como pueden ser los enlaces a scripts, el título o las hojas de estilo.
Es el primer hijo de un documento html.

De toda la información que contiene el head, la única que se va a ver en el navegador es el título o < title > < /title>.


**El cuerpo o body** < body > < /body >

El body contiene todo el contenido de la página, es decir todo lo que se va a ver en la página.

Estos elementos princiaples van dentro de la etiqueta <html> </html>.
Todas las etiquetas de un documento html lleva una apertura y un cierre.



>Las etiquetas más usadas en las páginas son:
> + < div > Es como un separador de contenido aunque en el navegador no muestra nada.
> + < h1 > Encabezado 1. Muestra en tamaño más grande la fuente y la pne en negrita por defecto. Así hasta < h6 >.
> + < p > Paragrapgh o párrafo.
> + < a > Ancle o ancla. Utilizada para insertar enlaces. Esta etqiueta lleva un atributo llamado "href" que es la ruta de ese enlace.
> + < ul > Lista desordenada.
> + < ol > Lista ordenada.
> + < li > List element o elemento de lista. Los elementos que van dentro de una lista.
> + < form > Etiqueta para formularios. Dentro se usa la etiqueta < label for=""> para darle un nombre a ese campo.Lleva también un atributo para guardar los datos introducidos en el formulario y el atributo required para hacerlo obligatorio
> + Lleva otro atributo llamado **method**, el cual puede ser ="get" o ="post" en caso de que tengamos un servidor y queramos hacer algo con esa info.
> < textarea > area de texto para introducir datos.
> < button > Agrega un botón. Con el atributo type se le puede decir si resetea o envía.

## 2. Tablas

>Las tablas se abren con la etiqueta < table>. Dentro de estas hay etiquetas para las filas, las columnas y los encabezados de estas.
> + < tr > Etiqueta table row, para las filas.
> + < th > Etiqueta table header para los encabezados o nombres de las filas
> + < td > Etiqueta table data, para los datos que irán dentro de la tabla.

## 3. Imágenes y vídeo
>La inserción de imágenes se realiza mediante la etiqueta < img > la cual lleva autocierre
> + < img src="ruta del archivo" alt="nombre que se uestra si la página no carga la imagen" atributos variados(width, heihgt)/>

>La inserción de vídeo se realiza mediante la etiqueta < video>
> + < video height=""px width=""px controls(para mostrar los controles) >
> + < source src="ruta del archivo" type="video/mp4" o el formato que sea /> Los formatos más usados son mp4,ogg y webm  


