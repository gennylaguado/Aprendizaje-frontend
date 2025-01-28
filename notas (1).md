# RoadMap Frontend - Angular

<div style="width: 100%; height: 300px; overflow: hidden; position: relative;">
  <img
    src="https://app.ashbyhq.com/api/images/user-content/89c1442c-bd9c-46be-a910-20b49b5d9ffc/1ca8c00e-a1bf-459a-9bde-4a23cee1f860/cixelyn_anime_designer_holding_a_webpage_1ec53089-c195-48e2-ad03-b0b5399ec35c.png"
    style="width: 100%; height: 100%; object-fit: cover; object-position: 50%; transform: scale(1);">
</div>

## Important Topics

1. ¿Qué es la web?

    La web es un sistema de información que se encuentra en internet y que se puede acceder a través de un navegador web.

2. ¿Como funciona un navegador web?

    Un navegador web es un software que se encarga de interpretar el código HTML, CSS y JavaScript de una página web y mostrarla en pantalla. Este proceso se realiza en 3 pasos:

     - El navegador recibe el código HTML de la página web.
     - El navegador interpreta el código HTML y crea un árbol de elementos (etiquetas HTML dentro de otras etiquetas HTML).
     - El navegador aplica los estilos CSS y ejecuta el código JavaScript.

3. ¿Qué es cliente y servidor?

    Un cliente es un dispositivo (celular, computador, tablet, etc.) que solicita información a un servidor (otro "computador" que contiene todo el codigo de la pagina). Y el servidor es el encargado de enviar la información solicitada por el cliente.

4. ¿Qué es un lenguaje?

    Un lenguaje es un conjunto de reglas y símbolos que se utilizan para comunicarse. En el caso de la programación, un lenguaje de programación es un conjunto de reglas y símbolos que se utilizan para escribir instrucciones que una computadora puede entender y ejecutar.

5. ¿Qué es un lenguaje de marcado?

    Un lenguaje de marcado es un lenguaje que se utiliza para definir la estructura y el contenido de un documento. HTML (HyperText Markup Language) es un lenguaje de marcado que se utiliza para crear páginas web. Es decir, el código escrito en ellos no se ejecuta, sino que se interpreta para mostrar la información en pantalla; mostrando casi tal cual como fue escrito.

6. ¿Qué es un lenguaje de estilos?

    Un lenguaje de estilos es un lenguaje que se utiliza para definir la apariencia y el diseño de un documento. CSS (Cascading Style Sheets) es un lenguaje de estilos que se utiliza para dar estilo a las páginas web. Es decir, se encarga de darle color, tamaño, posición, etc. a los elementos de la página.

> La siguiente página es muy recomendada para aprender sobre HTML y CSS: [W3Schools](https://www.w3schools.com/) hacerse amigo de esta página es una buena idea, porque a futuro de vez en cuando llegará a ella. Cuando ingrese a la página, en la parte superior encontrará un menú con las opciones de HTML, CSS, JavaScript, etc. Haga clic sobre HTML y CSS, dentro de ellas va a encontrar un menú lateral izquierdo con muchas cosas sobre HTML y CSS, como tutoriales, ejemplos, referencias, etc.

## Introducción a HTML

[HTML en 5 minutos](https://www.youtube.com/watch?v=EvKm8yhM7V8&ab_channel=DotDager)

Objetivo: Conocer la estructura y los elementos básicos del HTML.

1. ¿Qué es HTML?
2. Anatomía de un documento HTML.
3. Elementos básicos:
    - `<html>`, `<head>`, `<body>`
    - Títulos `<h1>` a `<h6>`
    - Párrafos `<p>`
    - Enlaces `<a>`
    - Imágenes `<img>`
4. Listas:
    - Ordenadas `<ol>`
    - desordenadas `<ul>`
5. Tablas: Estructura básica `<table>, <tr>, <td>, <th>`
6. Formularios:
    - Campos de texto `<input>`, botones `<button>`, selectores `<select>`
    - Atributos importantes como required, placeholder, etc.
7. Proyectos prácticos: (no requieren diseño y funcionalidad)
    - imitar un curriculum [ejemplo](https://www.youtube.com/watch?v=EqS6dp423CU&ab_channel=JuanCarlosMonegro)
    - Crear una página básica con texto, imágenes, y enlaces
    - Diseñar un formulario simple con campos de texto y un botón de envío.

## Introducción a CSS

Objetivo: Aprender a dar estilos a los elementos HTML.

1. ¿Qué es CSS?
2. Cómo enlazar CSS con HTML
    - inline `<anytag style="">`
    - intern `<style>`. ya sea dentro de la etiqueta body o head
    - archivo externo con `<link rel="stylesheet" href="styles.css">`
3. Selectores básicos:
   1. Selectores de elementos, clases (.class-name), e IDs (#id).

        ```css
        /* Element selector */
        p {
        color: red;
        }

        /* Class selector */
        .my-class {
        font-size: 20px;
        }

        /* ID selector */
        #my-id {
        background-color: blue;
        }
        ```

        > Nota: Los selectores de clases e IDs se utilizan para aplicar estilos a elementos específicos, mientras que los selectores de elementos se utilizan para aplicar estilos a todos los elementos de ese tipo (o sea, todas las etiquetas html de ese tipo).
        ---
        > Nota 2: Recordar el amarillo es el nombre de la etiqueta, clase o id; el azul es la propiedad y el rojo/verde es el valor de la propiedad.

   2. Selectores combinados

        ```css
        /* Elemento dentro de otro elemento */
        div p {
        color: red;
        }

        /*
        * El anterior selector se aplica a todos los elementos <p> que estén dentro de * un elemento <div>.
        */

        /* Elemento con una clase específica */
        div.my-class {
        font-size: 20px;
        }

        /*
        * El anterior selector se aplica a todos los elementos <div> que tengan la clase * "my-class".
        */

        /* Elemento con un ID específico */
        div#my-id {
        background-color: blue;
        }

        /*
        * El anterior selector se aplica a todos los elementos <div> que tengan el ID 
        * "my-id".
        */

        /* Elemento con una clase específica dentro de otro elemento */
        div p.my-class {
        font-size: 20px;
        }

        /*
        * El anterior selector se aplica a todos los elementos <p> que tengan la clase
        * "my-class" y que estén dentro de un elemento <div>.
        */

        /* Elemento con una clase específica directamente dentro de otro elemento */
        div > p.my-class {
        font-size: 20px;
        }

        /*
        * El anterior selector se aplica a todos los elementos <p> que tengan la clase
        * "my-class" y que estén directamente dentro de un elemento <div>.
        * Por directamente se entiende que no hay otros elementos entre el <div> y el <p> o que es la primera etiqueta <p> dentro del <div>.
        */
        ``

        > Nota: Los selectores combinados se utilizan para aplicar estilos a elementos específicos que cumplen con múltiples condiciones (lo que está en amarillo).

4. Propiedades esenciales:

    - Colores (color, background-color).
    - Tipografía (font-size, font-family, line-height).
    - Espaciado (margin, padding).
    - Bordes y sombras (border, box-shadow).
    - ...
    - [Referencia de propiedades CSS](https://carontestudio.com/blog/listado-de-propiedades-css/)

5. Sistema de cajas ([Box Model](https://www.w3schools.com/css/css_boxmodel.asp)): Conceptos de contenido, padding, border y margin.

6. Posicionamiento:
    - relative, absolute, fixed y static.
    - Uso de z-index.

7. Flexbox: [Referencia](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
   1. Contenedor y elementos flexibles.

        ```css
        .flex-container {
        display: flex;
        }

        .flex-item {
        flex: 1;
        }
        ```

   2. Propiedades como justify-content, align-items, y flex-wrap.

8. Grid Layout: [Referencia](https://css-tricks.com/snippets/css/complete-guide-grid/)

   1. Conceptos de filas y columnas.

        ```css
        .grid-container {
            display: grid;
        }
        ```

   2. Propiedades como grid-template-rows, grid-template-columns, y gap.

9. Proyectos prácticos:
    - Un currilum con estilos básicos.
    - Crear un diseño básico con Flex (una galería de imágenes de 3 columnas)

## CSS Un poco más avanzado

Objetivo: Aprender a dar estilos más avanzados a los elementos HTML.

1. Pseudo-clases y pseudo-elementos:
    - :hover, :active, :focus.
    - ::before, ::after.

        ```css
        /* Pseudo-clases */
        button:hover {
            background-color: red;
        }

        /*
        * El anterior selector se aplica a todos los elementos <a> cuando el cursor * del mouse está sobre ellos.
        */

        /* Pseudo-elementos */
        p::before {
            content: "Hola";
        }

        /*
        * El anterior selector inserta el texto "Hola" antes de cada elemento <p>.
        */

        p:first-child {
            color: red;
        }

        /* El anterior ejemplo selecciona el primer elemento <p> dentro de su contenedor. 
        */
        
        p:nth-child(2n) {
            color: blue;
        }

        /* El anterior ejemplo selecciona todos los elementos <p> que sean pares dentro de su contenedor. 
        */

        p:nth-child(odd) {
            color: green;
        }

        /* El anterior ejemplo selecciona todos los elementos <p> que sean impares dentro de su contenedor. 
        */

        p:nth-child(3) {
            color: yellow;
        }

        /* El anterior ejemplo selecciona el tercer elemento <p> dentro de su contenedor. 
        */

        /*
        para los anteriores ejemplos crear un contenedor con varios elementos <p> para que se pueda ver el efecto.
        */
        ```

2. Variables CSS. Se definen en el `:root` y se utilizan con `var()`. Son útiles para reutilizar valores en diferentes partes del código, como ejemplo el color principal de la página, el tamaño de la fuente, etc.

    ```css
    :root {
        --main-color: red;
    }

    p {
        color: var(--main-color);
    }
    ```

3. Animaciones y Transiciones:
    - `@keyframes` para definir animaciones.
    - `transition` para definir transiciones. [Referencia](https://www.w3schools.com/css/css3_transitions.asp)
    - `animation` para aplicar animaciones. [Referencia](https://www.w3schools.com/css/css3_animations.asp)

        ```css
        @keyframes example {
            0% {
                background-color: red;
            }
            100% {
                background-color: blue;
            }
        }

        div {
            animation: example 5s infinite;
        }

        button {
            transition: background-color 0.5s;
        }

        button:hover {
            background-color: red;
        }
        ```

4. Responsive Design:
    - Media queries.
    - Unidades relativas (%, vw, vh, em, rem). [Referencia](https://lacolmenatecnologica.com/elementor-academy-temas/cual-es-la-diferencia-entre-px-em-rem-vw-y-vh/)
    - [Referencia](https://www.w3schools.com/css/css_rwd_mediaqueries.asp)

        ```css
        @media screen and (max-width: 600px) {
            body {
                background-color: lightblue;
            }
        }

        div {
            width: 50%;
        }
        ```

5. Proyectos prácticos:
    - Crear un menú de navegación con animaciones.
    - Crear un portafolio con diseño responsive. [Ejemplo](https://www.youtube.com/watch?v=YMZmJfCOp_s&ab_channel=divcode)
    - Crear una galería de imágenes con transiciones (como que al pararse sobre una imagen, esa crece un poco, y al salir el mouse, la imagen vuelve a su tamaño original).
    - Hacer un diseño responsive de una página web (por ejemplo la galeria de imagenes anterior, que se vea bien cuando reduzca la pantalla).
    - slider de logos. [ejemplo](https://www.youtube.com/watch?v=zf7r0l5PCwE&ab_channel=CodeGlitch)
    - efecto de particulas en movimiento. [ejemplo](https://www.youtube.com/watch?v=fbn2aVaSb3E&ab_channel=SINERGIA)
    - luz ambiente a figura: [ejemplo](https://www.youtube.com/watch?v=nOdDtnHWaDo&ab_channel=OnlineTutorials)
    - [typewriter](https://www.youtube.com/shorts/fTOcWMD_5pk)
