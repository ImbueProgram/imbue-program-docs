# HTML

To build websites, you should know about HTML — the fundamental technology used to define the structure of a webpage. HTML is used to specify whether your web content should be recognized as a paragraph, list, heading, link, image, multimedia player, form, or one of many other available elements or even a new element that you define.

We encourage you to fully read [Learning Pathway MDN](https://developer.mozilla.org/en-US/docs/Learn/Html) (or at least the introduction to HTML). MDN will be a source of documentation for you along your career.

Go to [html5 introduction](https://www.freecodecamp.org/learn/responsive-web-design/basic-html-and-html5/) and complete all the lessons. This is the first module in the "Responsive Web design Certification" of [freeCodeCamp](https://www.freecodecamp.org/learn).

Once you are done, speak to your mentor and continue all the lessons until you finish the full certification. This is the first milestone to start filling your CV.

## Tutorials

### w3Schools
You can follow [this tutorial of HTML](https://www.w3schools.com/html/html_basic.asp) will be one good reference to solve your questions. 

### NodeSchool
You can also follow this nodeschool tutorial.
Open a terminal and type the next command
```
npm install -g learnyouhtml
```
Then type the next command: `learnyouhtml`


## Spanish 



## Fundamentos de HTML

HTML es el lenguaje básico del navegador. Está formado por etiquetas que te permiten construir o referenciar cualquier tipo de contenido.

#### Las etiquetas HTML
Las etiquetas son pequeñas piezas de código que contienen información. Existen más de 100 etiquetas en HTML y cada una cumple una función concreta que aporta diferente valor semántico. Es la forma que tenemos los desarrolladores web de decirle al navegador qué tipo de información estamos construyendo en cada momento y cómo debe ser interpretado.

Aunque más adelante veremos que todas las etiquetas son visualmente personalizables gracias a CSS, es muy importante que demos un buen uso de las mismas dependiendo de su finalidad.

La estructura de una etiqueta siempre es igual, salvo alguna pequeña excepción. Todas comienzan con la etiqueta de apertura, seguido del contenido y acabando con la etiqueta de cierre.

* **La etiqueta de apertura** se muestra comenzando con el símbolo `<` *(menor que)* + tipo de etiqueta + símbolo `>` *(mayor que)*. Ejemplo: `<p>`

* **El contenido** siempre se muestra de forma plana, sin necesidad de incorporar símbolos especiales. Ejemplo: `Contenido que quiero mostrar`

* **La etiqueta de cierre** es exactamente igual que la etiqueta de apertura pero, en este caso, añadimos el símbolo símbolo `/` *(slash)*. Siguiendo el ejemplo de apertura, la etiqueta de cierre quedaría así: `</p>`

Veamos una muestra completa siguiendo los ejemplos de apertura, contenido y cierre de los puntos anteriores, si queremos mostrar un párrafo (etiqueta `p` en HTML) lo haríamos así:
```
<p> Contenido que quiero mostrar </p>
```
Resultando en el navegador así:
> <p> Contenido que quiero mostrar</p>


#### La estructura HTML
La estructura de un archivo HTML es muy sencilla. De momento, quédate con tres etiquetas esenciales que componen un archivo de html:

* **`<html>`**:Es la etiqueta principal y raíz del lenguaje. Está encargada de designar, junto al formato de archivo (archivo.html), que el documento que estás creando es de tipo html. A su vez, `<html>` se divide en dos grandes etiquetas que veremos a continuación:

* **`<head>`**:La etiqueta `<head>` se utiliza para ubicar todos las etiquetas especiales que no son visibles de forma directa por el navegador. En ella se incluye información como metadatos, título de la página y es desde donde se enlazan otros ficheros web para complementar las funciones de HTML, como scripts de Javascript y hojas de estilos de CSS.

* **`<body>`**:La etiqueta `<body>`, al contrario que `<head>`, es donde ubicamos todos los elementos (tags) visibles por el usuario, como textos, imágenes, formularios, botones…



Esta es una lista de todas las etiquetas en HTML5 con una breve descripción:
<iframe width="100%" height="420" src="https://www.youtube.com/embed/dmovVa0jseU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

#### Your first line of HTML

La mejor forma de aprender un nuevo lenguaje, al igual que sucede con un idioma, es poniéndose manos a la obra y practicarlo lo máximo posible.

Abre tu editor de código (si aún no lo has instalado, Sigue [estas instrucciones](/program/frontend/setup/macOs.md "Editor de código").):
* Crea un nuevo archivo desde *Archivo > Nuevo archivo* o, mediante el atajo de teclado, Cmd+N en MacOS o Ctrl+N en Windows.

* Una vez creado, comprobarás que casi la única funcionalidad que te aporta el editor es la de escribir código. De momento no escribas nada, guarda el archivo en blanco desde *Archivo > Guardar como…* o Cmd+S / Ctrl+S en una carpeta nueva en tu escritorio o donde quieras. Ponle cualquier nombre pero añade la extensión `.html` al final del nombre del archivo.

* Abre el archivo que acabas de crear. Comúnmente, tu sistema operativo tratará de abrirlo desde tu navegador, si no fuera así, abre tu navegador (Google Chrome, Firefox, Edge…), ve a *Arhivo > Abrir archivo…* y selecciónalo.

En este punto, verás una web en blanco sin ningún contenido. A partir de ahora será nuestro lienzo donde empezar a construir.
