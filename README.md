# Curso de Preprocesadores CSS
2.-Conceptop básicos de CSS
===========================
CSS significa Cascading Style Sheets o su traducción al español Hojas de Estilo en Cascada.

Asignar reglas CSS a un documento HTML se puede hacer de varias formas:

  - Colocando las reglas en un documento *.css y relacionarlo al HTML usando la etiqueta
  - Colocando en el atributo style de cada elemento HTML las reglas para cada etiqueta
  - Colocando los estilos dentro de una etiqueta style dentro del head del documento.

Como su nombre lo dice siempre lee en cascada de arriba hacia abajo sobrescribiendo valores excepto los dados por el atributo style.

Un estilo CSS está formado por: selector, declaración => (propiedad y valor).

3.- Selectores de CSS
=====================
Los selectores nos sirven para seleccionar los diferentes elementos en una página web y aplicar estilos

Existen los siguientes tipos de selectores:

  - Selector universal " * " Sirve para agregar estilos a todos los elementos de la página. 
    Normalmente se utiliza para hacer “reset” de estilos.
  - Selector etiqueta. Aplica estilos a todos los elementos de ese tipo (p, h1, header etc.)
  - Selector id. Aplica estilos a un elemento único con ese Id, se recomienda hacer buen uso de 
    este selector.
  - Selector clase. Aplica estilos a todos los elementos con esa clase (el que más vas a usar).
  - Selector anidado. Aplica estilos a un elementos descendientes de otros elementos (no necesario 
    que sea hijo directo).
  - Selector hijo >. Aplica estilos a los elementos que sean hijos directos de otros.
  - Selector adyacente +. Aplica estilos al elemento adyacente.
  - Selector de atributo input[type=“number”]. Aplica estilos al elemento con el atributo 
    especificado.

La prioridad de un selector se determina por la suma de su contenido:

  - ID = 100
  - Clase = 10
  - Etiqueta = 1

A mayor la suma, mayor prioridad.

!important es un valor especial tiene un valor de un millón, nunca lo uses a menos que sea tu única opción como cuando no tienes acceso al código fuente.

4.- Introducción a los Preprocesadores
======================================
Un preprocesador es una herramienta que nos permite escribir pseudocódigo de forma modular, más fácil de rehusar, leer, y mantener. pseudocódigo que después será convertido a CSS o HTML estándar que el navegador entiende.

Gracias a los preprocesadores podemos extender las características de CSS y HTML al nivel de otros lenguajes de programación, permitiéndonos usar características como variables, funciones y mixins.

Las metodologías para estructurar código son sistemas preestablecidos, formales y bien documentados, que te ayudan a escribir y organizar código mantenible y escalable en sistemas grandes y complejos.

6.- Introducción a BEM
=====================
BEM es la metodología que vamos a usar a lo largo del curso. El objetivo de BEM es dividir lógicamente las piezas de las que se compone una web.

BEM establece que debemos usar clases para nuestro selectores, clases que se dividen en:

  - Bloques. Los bloques son nuestros contenedores más grandes que a su vez contienen elementos u 
    otros bloques.
  - Elementos. Los elementos siempre forman parte de un bloque, normalmente son los botones, 
    textos, imágenes etc.
  - Modificadores. Los modificadores se usan para establecer estilos diferentes a un mismo bloque o 
    elemento.

7.- Guías para creación y mantenimiento de código
=================================================
La meta de tener una guía de código es hacer que luzca como si una sola persona lo haya escrito para que se entendible por todo el equipo.

Para nuestro proyecto PlatziGames vamos a tener una guía en la que definimos:

    Ser consistentes con la indentación.
    Consistencia con espacios, corchetes, puntos y comas.
    Consistencia de números, de selectores y divisiones.
    Agrupaciones de propiedades.
    Uso de ID’s y clases.

8.- Introducción a Pug Preprocesadores de HTMl
==============================================

Pug es un generador de templates implementado con Javascript para Node.js y navegadores, que nos permite escribir un pseudocódigo limpio y fácil de leer que será compilado a HTML.

12.- Pug, preprocesador de HTML
===============================
Las variables no vienen de forma nativa en HTML pero con PUG podemos usarlas. En ellas almacenamos datos y los reutilizarlos en todo nuestro archivo HTML evitándonos tener que escribir lo mismo una y otra vez.Al incio de cualquier otro código.

-var titulo = "Sub-titulo Principal"
-var titulos = ["Titulo Principal", "Subtitulo 1", "Subtitulo 2", "Subtitulo 3"]

Un condicional nos permite evaluar cierta condición y bifurcar entre dos caminos dependiendo de si se cumple o no.

Un loop es un fragmento de código que va a ejecutar de forma repetitiva hasta que cumpla una condición. Lo podemos usar en una lista.