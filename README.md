# CPreprocesadoresCSS
Curso de Preprocesadores CSS

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