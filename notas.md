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
> + < form > Etiqueta para formularios. Dentro se usa la etiqueta < label for=""> para darle un nombre a ese campo.Lleva también un atributo para guardar
> los datos introducidos en el formulario y el atributo required para hacerlo obligatorio
> + Lleva otro atributo llamado **method**, el cual puede ser ="get" o ="post" en caso de que tengamos un servidor y queramos hacer algo con esa info.
> < textarea > area de texto para introducir datos.
> < button > Agrega un botón. Con el atributo type se le puede decir si resetea o envía.

## 1.2. Tablas

>Las tablas se abren con la etiqueta < table>. Dentro de estas hay etiquetas para las filas, las columnas y los encabezados de estas.
> + < tr > Etiqueta table row, para las filas.
> + < th > Etiqueta table header para los encabezados o nombres de las filas
> + < td > Etiqueta table data, para los datos que irán dentro de la tabla.

## 1.3. Imágenes y vídeo
>La inserción de imágenes se realiza mediante la etiqueta < img > la cual lleva autocierre
> + < img src="ruta del archivo" alt="nombre que se uestra si la página no carga la imagen" atributos variados(width, heihgt)/>

>La inserción de vídeo se realiza mediante la etiqueta < video>
> + < video height=""px width=""px controls(para mostrar los controles) >
> + < source src="ruta del archivo" type="video/mp4" o el formato que sea /> Los formatos más usados son mp4,ogg y webm

>La inserción de audio se realiza mediante la etiqueta < audio>
> + < audio controls >
> + < source src="ruta del archivo" type="audio/mp3" /> Los formatos más usados son mp3,wav,ogg.


# 2. Hoja de estilos Css
>La hojas de estilos Css se usan en las páginas para darle visosidad a los diferentes elementos.
>Si se va a usar una hoja de estilos o más de una  hay que referenciarlas en el head.
> + < link rel="stylesheet" href="ruta del archivo css que voy a usar">

+ Para crear una hoja de estilos, con el IDE que esté usando creo un documento.css y dentro de el voy escribiendo y modificando lo que necesito.

+ En el siguiente ejemplo se aplica estilo a las etiquetas de h1 y p con lo cual cada vez que aprezca esa etiqueta me aplicará todo lo que se encuentre dentro del estilo.
```
h1 {
    color: blue;
}

p {
    color:  red;
    font-size: 20pt;
}
```

+ Además de esto existen los **selectores**, que sirven para decir que dentro de un estilo que yo he creado para una etiqueta,
  una se comporte de una manera y otra se comporte de otra.
+ Para ello puede realizarse o bien por el id, o bien por el selector de clase.

```
Si se realiza por id:
Primero modificamos la línea del documento que deseamos agregandole un id.
<p id="parrafo de h1">Esto es un parrafo</p>
A continuación vamos al  documento Css y añadimos:

#parrafo-h1 {                    ⬅️ Con la almohadilla y el nombre del id uso el selector de **id**.
    color:aqua;
    font-size: 10pt;

}

Si se reliza por selector de clase:

<h1 class="encabezado">Trabajando con CSS</h1>
En el documento css en vez de usar la almohadilla usamos un **.**.


.encabezado{
    font-size: 24pt;
}

Existe también el selector universal, que es el asterisco * .
si yo tengo creada un clase y en el Css utilizo el siguiente código aplicaré ese estilo a todo lo que lleve
la clase con el nombre que le he dado.


*.nombre de clase{
    color:yellow;
}

En el caso de que quisiera aplicar un mismo estilo a varios elementos
.autor, .fecha, .ubicacion{
    font-style: italic;
    text-decoration: underline;

}

```
 + Hay diferentes formas de aplicar estilos. 
    + Con el archivo de hoja de estilos Css.Esta es la más recomendada.
    + Utilizando la etiqueta < style > dentro del head.Sino queda otra opción la usaremos.
    + Otra manera es importar un Css desde un URL.
    + Usando el atributo style.


>https://getbootstrap.com/  ⬅️ No necesita presentación.
https://purecss.io/start/ ⬅️ hoja de estilos.
https://coolors.co  ⬅️ nos permite crear paletas de colores aleatorias y copiar 
el código HEX del color para usarlo en la hoja de estilos CSS.

## 2.1 Padding, border y margin
+ Padding: es un espacio interno dentro del elemento o espacio entre el borde del contenedor
y el contenido del mismo.Si uso solo 
```
.tarjeta{
    border-style:solid;
    border-color: rgb(150,150,150);
    border-width: 1px;
    padding: 10px 20px   :arrow_left Si le paso 2 valores el primero es vertical y el segundo horizontal 
                         con tres elementos el tercero es para la parte de abajo.
}

```

+ El margin es el espacio que guarda el elemento con respecto al resto.Podemos configurarlo como el padding.

+ El border es la línea del elemento. Por llamarlo de alguna manera, el recuadro.

+ Para los tipos de fuente, podemos usar los predeterminados, o los de google 
https://fonts.google.com/ y añadirlos o bien a la hoja CSS o al documento.
