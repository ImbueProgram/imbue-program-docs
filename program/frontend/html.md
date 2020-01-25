# HTML

## Learn HTML
*Learn how to create your first web page.*

HTML es el lenguaje básico del navegador. Está formado por etiquetas que te permiten construir o referenciar cualquier tipo de contenido.

#### Las etiquetas
Las etiquetas son pequeñas piezas de código que contienen información. Existen más de 100 etiquetas en HTML y cada una cumple una función concreta que aporta diferente valor semántico. Es la forma que tenemos los desarrolladores web de decirle al navegador qué tipo de información estamos construyendo en cada momento y cómo debe ser interpretado.

Aunque más adelante veremos que todas las etiquetas son visualmente personalizables gracias a CSS, es muy importante que demos un buen uso de las mismas dependiendo de su finalidad.

La estructura de una etiqueta siempre es igual, salvo alguna pequeña excepción. Todas comienzan con la etiqueta de apertura, seguido del contenido y acabando con la etiqueta de cierre.

* La etiqueta de apertura se muestra comenzando con el símbolo `<` *(menor que)* + tipo de etiqueta + símbolo `>` *(mayor que)*. Ejemplo: `<p>`

* El contenido siempre se muestra de forma plana, sin necesidad de incorporar símbolos especiales. Ejemplo: `Contenido que quiero mostrar`

* La etiqueta de cierre es exactamente igual que la etiqueta de apertura pero, en este caso, añadimos el símbolo símbolo `/` *(slash)*. Siguiendo el ejemplo de apertura, la etiqueta de cierre quedaría así: `</p>`

Veamos una muestra completa siguiendo los ejemplos de apertura, contenido y cierre de los puntos anteriores, si queremos mostrar un párrafo (etiqueta `p` en HTML) lo haríamos así:
```
<p> Contenido que quiero mostrar </p>
```
Resultando en el navegador así:
> <p> Contenido que quiero mostrar</p>


#### La estructura HTML
La estructura de un archivo HTML es muy sencilla. De momento, quédate con tres etiquetas esenciales que componen un archivo de html:

* `<html>`:Es la etiqueta principal y raíz del lenguaje. Está encargada de designar, junto al formato de archivo (archivo.html), que el documento que estás creando es de tipo html. A su vez, `<html>` se divide en dos grandes etiquetas que veremos a continuación:

* `<head>`:La etiqueta `<head>` se utiliza para ubicar todos las etiquetas especiales que no son visibles de forma directa por el navegador. En ella se incluye información como metadatos, título de la página y es desde donde se enlazan otros ficheros web para complementar las funciones de HTML, como scripts de Javascript y hojas de estilos de CSS.

* `<body>`:La etiqueta `<body>`, al contrario que `<head>`, es donde ubicamos todos los elementos (tags) visibles por el usuario, como textos, imágenes, formularios, botones…



Esta es una lista de todas las etiquetas en HTML5 con una breve descripción:
<iframe width="100%" height="420" src="https://www.youtube.com/embed/dmovVa0jseU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>