# RoadMap Frontend - Básico hasta Angular

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

7. ¿Qué es un repositorio?

    Un repositorio es un lugar donde se almacena y se gestiona el código de un proyecto. Git es un sistema de control de versiones que se utiliza para gestionar los repositorios de código. Podemos imaginar un repositorio como una carpeta que contiene todos los archivos de un proyecto, y Git como una herramienta que nos permite llevar un control de los cambios realizados en esos archivos.

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

---

## Introducción a Git y GitHub

### Conceptos Básicos del Control de Versiones y Git

#### 1 ¿Qué es el Control de Versiones y Git?

Control de versiones: Permite rastrear cambios en archivos a lo largo del tiempo. Esto ayuda a colaborar con otros sin perder trabajo y a recuperar versiones anteriores.

- **Git:** Es un sistema de control de versiones distribuido, lo que significa que cada colaborador tiene una copia completa del historial de cambios. Es rápido, seguro y flexible.

#### 2 Instalación de Git y Configuración Inicial

- Descarga e instala Git desde [git-scm](https://git-scm.com/).
- Configura Git por primera vez
- [Guia](https://www.youtube.com/watch?v=JWnZvHOYBDc&ab_channel=CarlosMasterWeb)


Comandos y flags importantes:

`git config --global user.name "Tu Nombre"`

- Configura tu nombre para que aparezca en los commits.
- La flag --global asegura que la configuración aplica para todos los repositorios en tu máquina.

`git config --global user.email "tuemail@example.com"`

Asocia tu correo con los commits. Esto es importante para que los cambios se vinculen correctamente en plataformas como GitHub o GitLab.

Verifica tu configuración:

`git config --list`

Esto muestra todas las configuraciones de Git en tu máquina.

### Trabajando con un Repositorio Local

#### 1 Crear un Repositorio

Comando principal:

`git init`

Crea un repositorio local en la carpeta actual. Esto inicializa una carpeta .git oculta donde Git almacenará el historial de cambios. Es decir, si estamos en la carpeta C:/Users/Usuario/Proyectos, al ejecutar este comando, se creará una carpeta .git en la carpeta Proyectos.

Usa `ls -a` para confirmar que la carpeta .git fue creada.

#### 2 Agregar Archivos al Staging Area

Comando principal:

`git add <nombre_archivo>`

Mueve los archivos desde el Working Directory al Staging Area, preparándolos para el próximo commit.

Puedes usar el archivo específico (archivo.txt), o añadir todo con:

`git add .`

La flag `.` agrega todos los archivos modificados.

Ejemplo práctico:

Crea un archivo hola.txt con el comando:

`echo "Hola Git" > hola.txt`

Agrégalo al Staging Area:

`git add hola.txt`

Reto:

- Crear dos archivos (x.html, y.css).
- Usa `git add` para añadir solo uno al Staging Area y verifica con `git status`.

#### 3 Confirmar Cambios (Commit)

Comando principal:

`git commit -m "Mensaje del commit"`

- Un commit guarda los cambios del Staging Area en el historial de Git. Es importante añadir un mensaje descriptivo para recordar los cambios realizados. Podemos imaginar un commit como un "checkpoint" en el historial de cambios.
- La flag -m permite añadir un mensaje en una sola línea, que debe ser claro y específico. Por ejemplo, "Se agregó el navbar al proyecto".

#### 4 Ver el Historial

Comando principal:

`git log`

Log significa "registro" en inglés.

Muestra los commits realizados en el proyecto, incluyendo:
- Hash único del commit.
- Autor.
- Fecha.
- Mensaje del commit.

Flags útiles:

`git log --oneline`: Muestra los commits en una línea, más compacto.
`git log --graph`: Visualiza las ramas en forma gráfica.

#### 5 Ignorar Archivos con .gitignore

El archivo .gitignore contiene patrones para archivos o carpetas que no quieres rastrear.

Ejemplo:

Crea un archivo .gitignore

`echo "node_modules/" > .gitignore`

Esto lo que hace es agregar la palabra node_modules/ al archivo .gitignore, lo que significa que Git ignorará la carpeta node_modules,  se puede asumir que es una carpeta porque no tiene extensión (nota, hay algunos archivos que no tienen extensión, pero en general son carpetas).

Practica:

- Crea un archivo .gitignore y crear un archivo o carpeta.
- Verifica que Git muestra el archivo o carpeta con `git status`.
- Agregar el archivo o carpeta al archivo .gitignore.
- Verificar que Git ignore los archivos o carpetas con `git status`.

#### 6 Ver Cambios en Archivos

Comando principal:

`git diff`

Muestra los cambios realizados en los archivos desde el último commit.

- Las líneas en verde son las líneas añadidas.
- Las líneas en rojo son las líneas eliminadas.
- Las líneas en blanco son las líneas sin cambios.
- Para salir de la vista de cambios, presiona la tecla `q`.
- Para ver los cambios en un archivo específico, usa `git diff nombre_archivo`.
- Para ver los cambios entre dos commits, usa `git diff hash_commit_1 hash_commit_2`.
- Para ver los cambios en el Staging Area, usa `git diff --staged`.
- Para ver los cambios en un archivo específico en el Staging Area, usa `git diff --staged nombre_archivo`.
- Para ver los cambios entre dos ramas, usa `git diff rama_1 rama_2`.
- Para ver los cambios entre dos ramas en un archivo específico, usa `git diff rama_1 rama_2 nombre_archivo`.

Practica:

- Realiza cambios en un archivo y verifica los cambios con `git diff`.
- Agrega los cambios al Staging Area y verifica los cambios con `git diff --staged`.
- Realiza cambios en un archivo y crea un commit. Luego realiza más cambios y verifica los cambios con `git diff hash_commit`.

#### 7 Deshacer Cambios

Comandos principales:

`git checkout -- nombre_archivo`

- Descarta los cambios realizados en un archivo y lo restaura a la versión del último commit.
- Es importante tener cuidado con este comando, ya que los cambios no se pueden recuperar.
- Si el archivo está en el Staging Area, se puede usar `git checkout -- nombre_archivo` para descartar los cambios.
- Si el archivo no está en el Staging Area, se puede usar `git checkout HEAD -- nombre_archivo` para descartar los cambios.
- Si se quiere deshacer todos los cambios en todos los archivos, se puede usar `git checkout -- .`.

`git reset HEAD nombre_archivo`

- Mueve los cambios del Staging Area al Working Directory.
- Es útil si se añadió un archivo al Staging Area por error.
- Luego se puede usar `git checkout -- nombre_archivo` para descartar los cambios.
- Si se quiere deshacer todos los cambios en el Staging Area, se puede usar `git reset HEAD .`.
- Si se quiere deshacer un commit, se puede usar `git reset --soft HEAD~1` para deshacer el último commit y mantener los cambios en el Working Directory.

Practica:

- Realiza cambios en un archivo y agrega los cambios al Staging Area.
- Deshaz los cambios en el archivo con `git checkout -- nombre_archivo`.
- Realiza cambios en un archivo y agrega los cambios al Staging Area.
- Deshaz los cambios en el Staging Area con `git reset HEAD nombre_archivo`.
- Realiza cambios en un archivo y crea un commit.
- Deshaz el commit con `git reset --soft HEAD~1`.

#### 8 Ramas en Git

Una rama en Git es una línea de desarrollo independiente que permite trabajar en diferentes características del proyecto sin afectar la rama principal. Esto es útil para colaborar con otros desarrolladores, probar nuevas funcionalidades y mantener un historial de cambios organizado. POdemos imaginar una rama como una línea de tiempo paralela a la rama principal, donde se pueden realizar cambios sin afectar el código en la rama principal, y luego fusionar (merge) los cambios cuando estén listos.

Comandos principales:

`git branch`


- Muestra las ramas en el repositorio.
- La rama principal se suele llamar `main` o `master`.

`git branch nombre_rama`

- Crea una nueva rama con el nombre especificado.
- Para cambiar a la nueva rama, se usa `git checkout nombre_rama`.
- Para crear y cambiar a una nueva rama en un solo comando, se puede usar `git checkout -b nombre_rama`.

`git checkout nombre_rama`

- Cambia a la rama especificada.
- Para volver a la rama principal, se usa `git checkout main`.

#### 9 Fusionar Ramas

Fusionar o merge en Git combina los cambios de una rama en otra rama. Esto es útil para integrar nuevas funcionalidades, corregir errores y mantener un historial de cambios organizado. Se puede imaginar como unir dos líneas de tiempo paralelas en una sola línea de tiempo.

Comandos principales:

`git merge nombre_rama`

Esto fusiona los cambios de la rama especificada en la rama actual donde estamos ubicados.

### Clonar un Repositorio
Comando principal:

`git clone <URL>`

- Copia un repositorio remoto en tu máquina local.
- Normalmente se usa en URL un link https de un repositorio en GitHub, GitLab, etc. También se puede usar un link SSH, pero esto es un poco más avanzado.

Practica:

- Clona un repositorio público desde GitHub.

### Trabajar con un Repositorio Remoto

#### 1 Agregar un Repositorio Remoto

La idea de un repositorio Git es que se pueda llevar un control de versiones de lo desarrollado, pero también se pueda colaborar con otros desarrolladores. Para ello, se pueden subir los cambios a un repositorio remoto, como GitHub, GitLab, etc. Podemos imaginar un repositorio remoto como una copia del repositorio local en la nube, donde se pueden compartir los cambios con otros colaboradores.

Comando principal:

`git remote add origin <URL>`

- Asocia un repositorio remoto con tu repositorio local.
- Normalmente se usa origin como nombre del repositorio remoto, pero se puede usar otro nombre.
- Se suele usar en URL un link SSH o HTTPS de un repositorio en GitHub, GitLab, etc.

#### 2 Subir Cambios al Repositorio Remoto

Comandos principales:

`git push -u origin main`

- Sube los cambios del repositorio local al repositorio remoto.
- La flag -u establece la rama principal del repositorio remoto.
- Luego de usar -u una vez, se puede usar git push para subir los cambios en el futuro.
- Si se está en una rama diferente a main, se puede usar git push -u origin nombre_rama para subir los cambios de la rama actual.

#### 3 Descargar Cambios del Repositorio Remoto

Normalmente se trabaja en un proyecto con otros colaboradores, por lo que es importante mantenerse actualizado con los cambios realizados por otros. Para ello, se pueden descargar los cambios del repositorio remoto al repositorio local.

Comandos principales:

`git pull`

- Descarga los cambios del repositorio remoto al repositorio local.
- Es importante usar git pull antes de empezar a trabajar en un proyecto para tener la versión más reciente.
- Si se está en una rama diferente a main, se puede usar git pull origin nombre_rama para descargar los cambios de la rama especificada.
- Si se usa git pull y estamos ubicados en una rama x, se descargan los cambios de la rama x del repositorio remoto y quedan en la rama x del repositorio local.

### ¿Qué es un conflicto en Git?

Un conflicto en Git ocurre cuando dos ramas tienen cambios en la misma línea de un archivo. Esto puede suceder cuando dos colaboradores modifican el mismo archivo y suben los cambios al repositorio remoto. Git no puede determinar automáticamente cuál es la versión correcta, por lo que marca el conflicto y requiere que el usuario resuelva la situación.

### ¿Qué es GitHub?

GitHub es una plataforma en la nube que permite alojar repositorios Git. Es una herramienta esencial para colaborar con otros desarrolladores, compartir código, revisar cambios, y mantener un historial de versiones organizado. GitHub ofrece funcionalidades como solicitudes de extracción, problemas, proyectos, y más. Entonces podemos imaginar GitHub como una google drive o oneDrive pero para código y con muchas más funcionalidades. Podemos decir que Git es la herramienta y GitHub es la plataforma.

> Nota: GitLab es otra plataforma similar a GitHub, pero con algunas diferencias en funcionalidades y enfoque. Ambas son populares y ampliamente utilizadas en la comunidad de desarrollo. En la mayoria de las empresas, desarrollos o proyectos podrá encontrarse con Git, y alguna de estas dos plataformas.
 
Practica:

- Crear una cuenta en GitHub.
- Crear un repositorio en GitHub.
- Subir un proyecto a GitHub.
- Clonar un repositorio desde GitHub.
- Realizar cambios en el repositorio local y subirlos a GitHub.
- Descargar cambios del repositorio remoto a tu repositorio local.
- Crear una rama, hacer cambios, fusionar la rama y subir los cambios a GitHub.
- Es decir, jugar con git en el repositorio local e ir subiendo al remoto en github.

### ¿Como se suele trabajar con un repositorio?

Usualmente la forma de trabajar con un repositorio es la siguiente:

1. Se crea o clona un repositorio remoto que se encuentra en el GitHub o GitLab de la empresa o proyecto.
2. Se clona el repositorio en la máquina local con `git clone <URL>`.
3. Cuando se clona, quedamos ubicados en la rama principal, que suele ser `main`, `master`, `predev`.
4. Se crea una rama con `git branch nombre_rama` y se cambia a la rama con `git checkout nombre_rama`. Esto sucede porque normalmente no se trabaja directamente en la rama principal, sino en una rama secundaria, ya que las ramas principales suelen estar protegidas, y en caso de errores o cambios que se puedan demorar en realizar, entonces no afectan el código principal.
5. Se realizan los cambios en la rama secundaria, se agregan al Staging Area con `git add .`, o `git add nombre_archivo`, y se confirman con `git commit -m "Mensaje del commit"`.
6. Se suele revisar si hay cambios en la rama principal con `git pull origin main`, para tener la versión más reciente. Esto sucede porque a veces podemos demorarnos en realizar cambios y otros colaboradores pueden haber subido cambios al repositorio remoto durante ese tiempo.
7. Se fusionan los cambios de la rama principal en la rama secundaria con `git merge main`. Esto se hace para tener los cambios más recientes de la rama principal en la rama secundaria (nuestra rama de trabajo).
8. Se suben los cambios de la rama secundaria al repositorio remoto con `git push -u origin nombre_rama`. Esto se hace para subir los cambios al repositorio remoto y que otros colaboradores puedan ver los cambios y colaborar.
9. Se crea una solicitud de extracción (pull/merge request) en GitHub o GitLab para fusionar los cambios de la rama secundaria en la rama principal. Esto se hace para que otros colaboradores revisen los cambios y se aseguren de que no haya errores antes de fusionar los cambios en la rama principal. Antes de ser aceptado el pull request, los demás colaboradores todavia no tienen los cambios en su rama principal, es después de aceptado que los demás colaboradores pueden descargar los cambios con `git pull origin main`.

## JavaScript

![Descripción de la imagen](https://raw.githubusercontent.com/cat-milk/Anime-Girls-Holding-Programming-Books/master/Javascript/Maya_Yamato_Holding_Javascript_For_Absolute_Beginners.png)

> Nota: He agregado muchos enlaces a videos, esto con el fin de encontrar una explicación más visual, pero sucede que a veces los videos muestran los conceptos en otros lenguajes de programación, pero esto es lo bonito de la programación, que los conceptos son casi siempre los mismos y solo cambia la sintaxis a usar.

### Introducción a JavaScript

JavaScript es un lenguaje de programación que se utiliza para crear páginas web interactivas. Es un lenguaje de programación de alto nivel, interpretado y orientado a objetos. JavaScript se ejecuta en el navegador web del usuario, lo que permite interactuar con los elementos de la página, realizar cálculos, enviar y recibir datos, y mucho más.

- **¿Qué diferencia a un lenguaje de programación de un lenguaje de marcado?:** Un lenguaje de programación se utiliza para escribir instrucciones que una computadora puede entender y ejecutar, mientras que un lenguaje de marcado se utiliza para definir la estructura y el contenido de un documento. Una diferencia clave es que un lenguaje de programación se ejecuta, mientras que un lenguaje de marcado se interpreta. Con un lenguaje de programación, se pueden realizar cálculos, tomar decisiones, y realizar acciones, mientras que con un lenguaje de marcado, se definen los elementos de la página, como títulos, párrafos, imágenes, etc.

- **¿Qué es un lenguaje de alto nivel?:** Un lenguaje de alto nivel es un lenguaje de programación que se asemeja al lenguaje humano y es fácil de leer y escribir. Los lenguajes de alto nivel se utilizan para escribir programas que se ejecutan en una computadora. Algunos ejemplos de lenguajes de alto nivel son Python, Java, C++, y JavaScript.

- **¿Qué significa que un lenguaje de programación sea interpretado?:** Un lenguaje de programación interpretado es un lenguaje que se ejecuta línea por línea, en tiempo real, por un intérprete. Esto significa que el código se ejecuta a medida que se escribe, sin necesidad de compilarlo antes de ejecutarlo. JavaScript es un lenguaje de programación interpretado, lo que significa que se puede escribir y ejecutar en un navegador web sin necesidad de compilarlo.

### ¿Por qué JavaScript?

JavaScript es uno de los lenguajes de programación más populares y ampliamente utilizados en el mundo. Es un lenguaje versátil que se puede utilizar para crear aplicaciones web, juegos, aplicaciones móviles, servidores, y mucho más. JavaScript es un lenguaje de programación esencial para cualquier desarrollador web, ya que permite crear páginas web interactivas y dinámicas.

#### Recomendaciones

- [¿Qué es la programación](https://www.youtube.com/watch?v=a7eznAouNak&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=1)
- [JavaScript en 5 minutos](https://youtu.be/FuCiNVP88pc?si=y3s5ILbUW8uf2bDq)

### Uso de la consola del navegador

La consola del navegador es una herramienta que permite interactuar con el código JavaScript de una página web. Se puede utilizar para depurar código, probar funciones, y ver mensajes de error. La consola del navegador se puede abrir en la mayoría de los navegadores web presionando F12 o haciendo clic derecho en la página y seleccionando "Inspeccionar".

- ¿Qué es depurar código?: Depurar código es el proceso de identificar y corregir errores en un programa. La consola del navegador es una herramienta útil para depurar código JavaScript, ya que muestra mensajes de error y permite ejecutar código en tiempo real. Podemos decir que depurar es como ir buscando errores en el código, y corregirlos para que el programa funcione correctamente.

Para escribir código JavaScript, se puede abrir la consola del navegador y escribir el código directamente en la consola. Por ejemplo, se puede escribir `console.log("Hola, mundo")` y presionar Enter para ver el mensaje "Hola, mundo" en la consola.

>Por otra parte, lo usual es escribir el código JavaScript en un archivo con la extensión .js y enlazarlo con el archivo HTML con la etiqueta `<script src="archivo.js"></script>`. De esta forma, el código JavaScript se ejecuta cuando se carga la página web.

### Sintaxis básica

La sintaxis de un lenguaje de programación se refiere a las reglas y estructuras que se utilizan para escribir código. Es decir, el texto que se escribe en un lenguaje de programación debe seguir ciertas reglas para que la computadora pueda entenderlo y ejecutarlo correctamente. Así como en un idioma se utilizan reglas gramaticales para formar oraciones, en un lenguaje de programación se utilizan reglas de sintaxis para formar instrucciones.
Algunos conceptos básicos de la sintaxis de JavaScript son:

#### Comentarios

Los comentarios son texto que se utiliza para explicar el código y no se ejecutan. En JavaScript, los comentarios se pueden escribir de dos formas: con `//` para comentarios de una línea y con `/* */` para comentarios de varias líneas.

```javascript
// Este es un comentario de una línea

/*
Este es un comentario
de varias líneas
*/
```

#### Variables

Las variables se utilizan para almacenar valores en un programa. En JavaScript, se pueden declarar variables con la palabra clave `let`, `const`, o `var`, seguida del nombre de la variable y el valor que se le asigna.

```javascript
let nombre = "Juan";
const edad = 25;
var altura = 1.75;
```

cosas a tener en cuenta:

- let: se utiliza para declarar variables que pueden cambiar de valor. Es decir, se pueden reasignar o cambiar su valor en otro momento del programa.
- const: se utiliza para declarar variables que no pueden cambiar de valor. Es decir, una vez que se asigna un valor a una variable constante, no se puede cambiar.
- var: se utilizaba en versiones antiguas de JavaScript para declarar variables, pero en la actualidad se recomienda utilizar let y const en su lugar.
- Estas palabras claves deben ser en minúsculas y no se pueden utilizar como nombres de variables.
- Los nombre de las variables suelen ser en minúsculas, y si son compuestas, se separan con guiones bajos `_` o con notación camelCase. No pueden empezar con números, ni contener espacios, ni caracteres especiales, ni palabras reservadas (por ejemplo, let, const, var, function, etc.).
- Las variables deben ser unicas, es decir, no se pueden declarar dos variables con el mismo nombre en el mismo ámbito o alcance (esto se verá más adelante).

#### Recomendaciones

- [¿Qué es una variable?](https://www.youtube.com/watch?v=kZfuJvkdcHU&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=2)

#### Tipos de datos

Los tipos de datos en JavaScript se utilizan para representar diferentes tipos de valores, como números, cadenas de texto, booleanos, objetos, arreglos, y más. Algunos tipos de datos básicos en JavaScript son:

```javascript
let numero = 10; // Número entero
let decimal = 3.14; // Número decimal
let texto = "Hola"; // Cadena de texto
let esVerdadero = true; // Valor booleano
let persona = {nombre: "Juan", edad: 25}; // Objeto
let colores = ["rojo", "verde", "azul"]; // Arreglo
```

cosas a tener en cuenta:

- Los números en JavaScript pueden ser enteros o decimales.
- Las cadenas de texto se escriben entre comillas simples o dobles.
- Los valores booleanos pueden ser `true` o `false`.
- Los objetos se utilizan para almacenar múltiples valores en una sola variable. Se definen con llaves `{}` y se acceden por clave, es decir, `persona.nombre` o `persona.edad`.
- Los arreglos se utilizan para almacenar múltiples valores en una sola variable, y se acceden por índice. Se definen con corchetes `[]` y se acceden por posición, es decir, `colores[0]` o `colores[1]`.
- JavaScript es un lenguaje de programación dinámico, lo que significa que no es necesario declarar explícitamente el tipo de dato de una variable. El tipo de dato se infiere automáticamente en función del valor asignado a la variable.
- JavaScript es un lenguaje de programación débilmente tipado, lo que significa que las variables pueden cambiar de tipo durante la ejecución del programa. Por ejemplo, una variable que almacena un número entero puede cambiar a una cadena de texto en otro momento del programa.

#### Recomendaciones

- [Entender un array o arreglo, el de los []](https://www.youtube.com/watch?v=k24J92Hod50)
- [Otra explicación de los array o arreglos](https://www.youtube.com/watch?v=_FsRvYZNbnc&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=7)

### Operadores básicos

Los operadores en JavaScript se utilizan para realizar operaciones matemáticas, comparaciones, asignaciones, y más. Algunos operadores básicos en JavaScript son:

#### Operadores aritméticos

Se utilizan para realizar operaciones matemáticas, como suma, resta, multiplicación, división, y más.

```javascript
let suma = 10 + 5; // Suma
let resta = 10 - 5; // Resta
let multiplicacion = 10 * 5; // Multiplicación
let division = 10 / 5; // División
let modulo = 10 % 5; // Módulo
```

cosas a tener en cuenta:

- El operador de suma `+` se puede utilizar para concatenar cadenas de texto.
- El operador de módulo `%` devuelve el resto/residuo de la división entre dos números.
- Los operadores aritméticos siguen las reglas de precedencia matemática, es decir, se evalúan en un orden específico. Por ejemplo, la multiplicación y la división tienen mayor precedencia que la suma y la resta.
- Se pueden utilizar paréntesis `()` para cambiar el orden de evaluación de los operadores.
- Los operadores aritméticos se pueden combinar con variables y valores para realizar cálculos.
- Los operadores aritméticos se pueden utilizar con números enteros y decimales.
- Los operadores aritmeticos se pueden utilizar para varios números, no solo dos, por ejemplo, `10 + 5 - 3`.

#### Operadores de comparación

Se utilizan para comparar dos valores y devolver un valor booleano `true` o `false`.

```javascript
let esIgual = 10 == 5; // Igual a (compara el valor) ¿10 es igual a 5?
let esDiferente = 10 != 5; // Diferente de (compara el valor) ¿10 es diferente de 5?
let esMayor = 10 > 5; // Mayor que (compara el valor) ¿10 es mayor que 5?
let esMenor = 10 < 5; // Menor que (compara el valor) ¿10 es menor que 5?
let esMayorIgual = 10 >= 5; // Mayor o igual que (compara el valor) ¿10 es mayor o igual que 5?
let esMenorIgual = 10 <= 5; // Menor o igual que (compara el valor) ¿10 es menor o igual que 5?

// texto
let esIgualTexto = "hola" == "mundo"; // ¿"hola" es igual a "mundo"?

// booleanos
let esIgualBooleano = true == false; // ¿true es igual a false?
```

cosas a tener en cuenta:

- El operador de igualdad `==` compara los valores de dos variables, pero no compara el tipo de dato. Por ejemplo, `10 == "10"` devuelve `true`.
- El operador de desigualdad `!=` devuelve `true` si los valores de dos variables son diferentes.
- Se pueden utilizar los operadores de comparación con números, cadenas de texto, booleanos, y más.

#### Operadores lógicos

Se utilizan para combinar dos o más expresiones lógicas y devolver un valor booleano `true` o `false`.

```javascript
let menor = 10 < 5 && 5 < 3; // Y lógico (AND) ¿10 es menor que 5 y 5 es menor que 3?
let mayor = 10 > 5 || 5 < 3; // O lógico (OR) ¿10 es mayor que 5 o 5 es menor que 3?
let y = true && false; // Y lógico (AND) ¿true y false?
let o = true || false; // O lógico (OR) ¿true o false?
let no = !true; // Negación lógica (NOT) ¿no true?
```

cosas a tener en cuenta:

- El operador `&&` devuelve `true` si ambas expresiones son verdaderas.
- El operador `||` devuelve `true` si al menos una de las expresiones es verdadera.
- El operador `!` devuelve `true` si la expresión es falsa y `false` si la expresión es verdadera. Es decir, invierte el valor de la expresión.
- Los operadores lógicos se pueden combinar con operadores de comparación para realizar operaciones más complejas. Por ejemplo, `10 > 5 && 5 < 3` devuelve `false`, porque la primera expresión es verdadera y la segunda es falsa, entonces como ambas deben ser verdaderas para que el `&&` devuelva `true`, entonces devuelve `false`.

#### Operadores de asignación

Se utilizan para asignar un valor a una variable.

```javascript
let x = 10; // Asignación simple
let y = 5;
y = y + 3; // Asignación de suma (y = y + 3)
y += 3; // Asignación de suma (y = y + 3) Forma abreviada
y = y - 3; // Asignación de resta (y = y - 3)
y -= 3; // Asignación de resta (y = y - 3) Forma abreviada
y *= 3; // Asignación de multiplicación (y = y * 3)
y /= 3; // Asignación de división (y = y / 3)
y %= 3; // Asignación de módulo (y = y % 3)
y = y + 1; // Asignación de sumar uno
y++; // Asignación de sumar uno

```

cosas a tener en cuenta:

- Los operadores de asignación se pueden combinar con operadores aritméticos para realizar operaciones matemáticas y asignar el resultado a una variable.

#### Recomendaciones

- [¿Qué son los condicionales?](https://www.youtube.com/watch?v=RaWfeVgkWbE&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=3)

### Estructuras de control

Las estructuras de control en JavaScript se utilizan para controlar el flujo de un programa y tomar decisiones en función de ciertas condiciones. En palabras simples, las estructuras de control permiten ejecutar ciertas instrucciones si se cumple una condición, o ejecutar otras instrucciones si no se cumple la condición. Algunas estructuras de control básicas en JavaScript son:

#### Estructura `if`

Se utiliza para ejecutar un bloque de código si se cumple una condición.

```javascript
let edad = 18;

if (edad >= 18) {
    console.log("Eres mayor de edad");
}
```

Esto significa que si la variable `edad` es mayor o igual a 18, se mostrará el mensaje "Eres mayor de edad" en la consola.

cosas a tener en cuenta:

- La condición se evalúa entre paréntesis `()`.
- El bloque de código se encierra entre llaves `{}`.
- Si la condición es verdadera, se ejecuta el bloque de código. Si la condición es falsa, no se ejecuta el bloque de código.
- Se pueden utilizar operadores de comparación y operadores lógicos en la condición.
- Se pueden anidar múltiples estructuras `if` para realizar múltiples comprobaciones.
- Se puede utilizar la estructura `if` sin llaves si el bloque de código es una sola línea.

#### Estructura `if-else`

Se utiliza para ejecutar un bloque de código si se cumple una condición, y otro bloque de código si no se cumple la condición.

```javascript
let edad = 16;

if (edad >= 18) {
    console.log("Eres mayor de edad");
} else {
    console.log("Eres menor de edad");
}
```

Esto significa que si la variable `edad` es mayor o igual a 18, se mostrará el mensaje "Eres mayor de edad" en la consola, y si no se cumple la condición, se mostrará el mensaje "Eres menor de edad".

#### Estructura `if-else if-else`

Se utiliza para ejecutar un bloque de código si se cumple una condición, otro bloque de código si se cumple otra condición, y un tercer bloque de código si no se cumple ninguna de las condiciones anteriores.

```javascript
let hora = 14;

if (hora < 12) {
    console.log("Buenos días");
} else if (hora < 18) {
    console.log("Buenas tardes");
} else {
    console.log("Buenas noches");
}
```

Esto significa que si la variable `hora` es menor a 12, se mostrará el mensaje "Buenos días" en la consola, si la variable `hora` es menor a 18, se mostrará el mensaje "Buenas tardes", y si no se cumple ninguna de las condiciones anteriores, se mostrará el mensaje "Buenas noches".

cosas a tener en cuenta:

- Se pueden utilizar múltiples bloques `else if` para realizar múltiples comprobaciones.
- La estructura `if-else if-else` se evalúa de arriba hacia abajo, y se ejecuta el primer bloque de código cuya condición sea verdadera.
- Se puede utilizar la estructura `if-else if-else` sin el bloque `else` si no se necesita un bloque de código para la condición que no se cumple.

#### Estructura `switch`

Se utiliza para ejecutar un bloque de código en función de una expresión.

```javascript
let dia = "lunes";

switch (dia) {
    case "lunes":
        console.log("Hoy es lunes");
        break;
    case "martes":
        console.log("Hoy es martes");
        break;
    case "miércoles":
        console.log("Hoy es miércoles");
        break;
    default:
        console.log("Hoy es otro día");
}
```

Esto significa que si la variable `dia` es "lunes", se mostrará el mensaje "Hoy es lunes" en la consola, si la variable `dia` es "martes", se mostrará el mensaje "Hoy es martes", si la variable `dia` es "miércoles", se mostrará el mensaje "Hoy es miércoles", y si no se cumple ninguna de las condiciones anteriores, se mostrará el mensaje "Hoy es otro día".

cosas a tener en cuenta:

- La estructura `switch` se utiliza para comparar una expresión con múltiples casos y ejecutar un bloque de código en función del caso que se cumpla.
- Se utiliza la palabra clave `case` para definir los casos y la palabra clave `break` para salir de la estructura `switch`.
- Se puede utilizar la palabra clave `default` para definir un caso por defecto que se ejecuta si no se cumple ninguno de los casos anteriores.
- La estructura `switch` es útil cuando se tienen múltiples casos que se pueden comparar con una sola expresión.
- Se puede utilizar la estructura `switch` sin la palabra clave `default` si no se necesita un caso por defecto.
- Es muy importante recordar el `break` al final de cada `case`, ya que si no se pone, se ejecutarán todos los `case` que estén debajo del `case` que se cumpla.
- Es muy similar a `if-else if-else`, pero se utiliza cuando se tienen muchos casos que se pueden comparar con una sola expresión.

#### Recomendaciones

- [Explicación del switch](https://www.youtube.com/watch?v=zPKylS8ifuI)
- [Otra explicación del switch](https://www.youtube.com/watch?v=Cywj2rx2AMc&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=4)

#### Estructura `for`

Se utiliza para ejecutar un bloque de código un número específico de veces.

```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

Esto significa que se mostrará en la consola los números del 0 al 4, ya que la variable `i` se inicializa en 0, se incrementa en 1 en cada iteración, y se ejecuta el bloque de código mientras `i` sea menor a 5.

cosas a tener en cuenta:

- La estructura `for` se compone de tres partes: la inicialización, la condición, y la actualización.
- La inicialización se ejecuta una vez al principio del bucle y se utiliza para inicializar la variable de control.
- La condición se evalúa antes de cada iteración y se utiliza para determinar si se ejecuta el bloque de código.
- La actualización se ejecuta al final de cada iteración y se utiliza para actualizar la variable de control.
- Se pueden utilizar múltiples variables en la inicialización, la condición, y la actualización.
- Se pueden utilizar operadores aritméticos y lógicos en la condición.
- Se puede utilizar la estructura `for` para recorrer arreglos, realizar cálculos, y más.

#### Recomendaciones

- [Explicación de for](https://www.youtube.com/watch?v=7bO5wlqeeEI&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=6)
- [Otra explicación de for](https://www.youtube.com/watch?v=ywIVQBaPRYk)

#### Estructura `while`

Se utiliza para ejecutar un bloque de código mientras se cumpla una condición.

```javascript
let i = 0;

while (i < 5) {
    console.log(i);
    i++;
}
```

Esto significa que se mostrará en la consola los números del 0 al 4, ya que la variable `i` se inicializa en 0, se incrementa en 1 en cada iteración, y se ejecuta el bloque de código mientras `i` sea menor a 5.

cosas a tener en cuenta:

- La estructura `while` se compone de una condición y un bloque de código.
- La condición se evalúa antes de cada iteración y se utiliza para determinar si se ejecuta el bloque de código.
- El bloque de código se ejecuta mientras la condición sea verdadera.
- Se pueden utilizar operadores aritméticos y lógicos en la condición.
- Se puede utilizar la estructura `while` para realizar cálculos, interactuar con el usuario, y más.
- Es muy importante tener cuidado con los bucles infinitos, es decir, bucles que nunca terminan, ya que pueden hacer que el programa se bloquee o se vuelva muy lento.
- Es muy similar a `for`, pero se utiliza cuando no se sabe cuántas veces se va a ejecutar el bloque de código.

#### Recomendaciones

- [Explicación de while](https://www.youtube.com/watch?v=cuFSVjo9oi0)
- [Otra explicación de while](https://www.youtube.com/watch?v=0h_srypSheg&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=5)

#### Estructura `do-while`

Se utiliza para ejecutar un bloque de código al menos una vez, y luego repetirlo mientras se cumpla una condición.

```javascript
let i = 0;

do {
    console.log(i);
    i++;
} while (i < 5);
```

Esto significa que se mostrará en la consola los números del 0 al 4, ya que la variable `i` se inicializa en 0, se incrementa en 1 en cada iteración, se ejecuta el bloque de código al menos una vez, y se repite mientras `i` sea menor a 5.

cosas a tener en cuenta:

- La estructura `do-while` se compone de un bloque de código y una condición.
- El bloque de código se ejecuta al menos una vez, y luego se repite mientras la condición sea verdadera.
- La condición se evalúa al final de cada iteración, lo que garantiza que el bloque de código se ejecute al menos una vez.

### Retos

- Realizar un programa que muestre los números del 1 al 10 en la consola.

```javascript 
let number = 1;

while (numero <= 10) {
  console.log(numero);
  numero++;
}
```
- Realizar un programa que determine si un número es par o impar.

```javascript	
let numero = 3;
let modulo = numero % 2; // Para saber si es par
console.log(numero);
if (modulo == 0) {
  console.log("Es par");
} else {
  console.log("Es impar");
}
```

- Realizar un programa que muestre los números pares del 1 al 10 en la consola.

```javascript
for (let index = 1; index <= 10; index++) {
  let modulo = index % 2;
  if (modulo == 0) {
    console.log(index);
  } 
}
```

- Realizar un programa que muestre los números impares del 1 al 10 en la consola.

```javascript
for (let index = 1; index <= 10; index++) {
  let modulo = index % 2;
  if (modulo != 0) {
    console.log(index);
  } 
}
```

- Realizar un programa que muestre los números del 10 al 1 en la consola.

```javascript
for (let index = 10; index >= 1; index--) {
  console.log(index);
}
```

- Realizar un programa que muestre los números pares del 10 al 1 en la consola.
- 
```javascript
for (let index = 10; index >= 1; index--) {
  if (index % 2 == 0) {
    console.log(index);
  } 
}
```

- Realizar un programa que muestre los números impares del 10 al 1 en la consola.
- Simular un mini cajero automatico que de un mensaje según el saldo del usuario, por ejemplo, si el saldo es mayor a 1000, mostrar "Saldo suficiente", si el saldo es menor a 1000 y mayor a 500, mostrar "Saldo insuficiente", si el saldo es menor a 500, mostrar "Saldo crítico".

#### Recomendaciones

- [JavaScript en 4 minutos](https://www.youtube.com/watch?v=HyAoI3gxoLI) Este video quiero lo vea y ya, no le pido que lo entienda del todo, ya que hay conceptos que no he explicado, pero es para que se vaya familiarizando con el lenguaje, no hay excusa.

```javascript
let saldo = 1000

if (saldo > 1000) {
  console.log("Saldo suficiente")
} else if (Saldo>500) {
    console.log("Saldo insuficiente")
} else {
    console.log("Saldo crítico")
}
```

### Funciones

Las funciones en JavaScript se utilizan para encapsular un bloque de código y reutilizarlo en diferentes partes de un programa. Una función puede aceptar parámetros, realizar operaciones, y devolver un valor si es necesario. Algunos conceptos básicos de las funciones en JavaScript son:

#### Declaración de funciones

Se utiliza para definir una función y especificar los parámetros y el bloque de código que se ejecuta cuando se llama a la función.

```javascript
function saludar() {
    console.log("Hola, mundo");
}

saludar(); // Llama a la función saludar
```

Esto significa que al llamar a la función `saludar`, se mostrará el mensaje "Hola, mundo" en la consola.

cosas a tener en cuenta:

- La palabra clave `function` se utiliza para declarar una función.
- El nombre de la función se utiliza para llamar a la función en otras partes del programa.
- Los paréntesis `()` se utilizan para definir los parámetros de la función.
- El bloque de código de la función se encierra entre llaves `{}`.
- La función se ejecuta cuando se llama a la función con el nombre y los paréntesis.
- Se pueden utilizar múltiples funciones en un programa para realizar diferentes tareas.
- Las funciones se pueden llamar desde otras funciones, desde eventos, desde bucles, y más.
- Las funciones deben ser unicas, es decir, no se pueden declarar dos funciones con el mismo nombre en el mismo ámbito o alcance (esto se verá más adelante).

#### Parámetros de funciones

Se utilizan para pasar valores a una función y realizar operaciones con esos valores.

```javascript
function sumar(a, b) {
    let resultado = a + b;
    console.log(resultado);
}

sumar(5, 3); // Llama a la función sumar con los valores 5 y 3
sumar(10, 2); // Llama a la función sumar con los valores 10 y 2
```

Esto significa que al llamar a la función `sumar` con los valores 5 y 3, se mostrará el resultado de la suma en la consola, y al llamar a la función `sumar` con los valores 10 y 2, se mostrará el resultado de la suma en la consola.

cosas a tener en cuenta:

- Los parámetros se definen entre paréntesis `()` y se separan por comas `,`.
- Los parámetros se utilizan para pasar valores a una función y realizar operaciones con esos valores.
- Los parámetros se pueden utilizar en el bloque de código de la función como variables locales.
- Se pueden utilizar múltiples parámetros en una función para realizar operaciones más complejas.
- Los valores que se pasan a una función se llaman argumentos, es decir, se les dice parámetros cuando se define la función, y argumentos cuando se llama a la función.

Acá se introdujo un nuevo termino que es "variables locales". Antes de esta sección, se habló de variables, que son como "cajas" (más adelante cambiará el concepto) que se utilizan para almacenar valores en un programa. Lo que sucedía es que esas variables se podían utilizar en cualquier parte del programa, es decir, eran "globales". Pero en este caso, las variables locales son variables que solo se pueden utilizar dentro de una función, es decir, solo son accesibles dentro de la función en la que se declaran. Esto es útil para evitar conflictos de nombres y mantener el código organizado. Por ejemplo, si se declara una variable `resultado` dentro de una función, solo se puede utilizar dentro de esa función, y no se puede acceder desde otras partes del programa. En la estructura `for` y `while` también se utilizan variables locales, ya que las variables de control solo se pueden utilizar dentro del bucle.

#### Recomendaciones

- [Otra explicación de funciones](https://www.youtube.com/watch?v=AzeyTH_AjFE)
- [¿Qué es una función?](https://www.youtube.com/watch?v=XCHKaSNjoak&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=9)
- [Otra explicación de funciones](https://www.youtube.com/watch?v=MiH3pbP4EFc)

#### Scope de variables

El scope de una variable se refiere a la visibilidad y accesibilidad de la variable en un programa. En JavaScript, las variables pueden tener scope global o scope local, lo que significa que pueden ser accesibles desde cualquier parte del programa o solo desde una parte específica del programa.

```javascript
let global = "Variable global";

function funcion() {
    let local = "Variable local";
    console.log(global); // Accede a la variable global
    console.log(local); // Accede a la variable local
}

console.log(global); // Accede a la variable global
console.log(local); // Error: la variable local no está definida
```

#### Retorno de funciones (return)

Se utiliza para devolver un valor desde una función y utilizarlo en otras partes del programa. Por ejemplo, se puede utilizar una función para realizar un cálculo y devolver el resultado.

```javascript
function sumar(a, b) {
    let resultado = a + b;
    return resultado;
}

let total = sumar(5, 3); // Llama a la función sumar y guarda el resultado en la variable total
console.log(total); // Muestra el resultado en la consola
```

Esto significa que al llamar a la función `sumar` con los valores 5 y 3, se devolverá el resultado de la suma, y se guardará en la variable `total`, que luego se mostrará en la consola.

cosas a tener en cuenta:

- La palabra clave `return` se utiliza para devolver un valor desde una función.
- El valor devuelto por la función se puede guardar en una variable y utilizarlo en otras partes del programa.
- Se puede utilizar `return` para devolver cualquier tipo de valor, como números, cadenas de texto, booleanos, objetos, arreglos, y más.

#### Funciones flecha (arrow functions)

Las funciones flecha son una forma más corta y concisa de definir funciones en JavaScript. Se utilizan para simplificar la sintaxis y reducir la cantidad de código necesario para definir una función.

```javascript
// Función tradicional
function saludar() {
    console.log("Hola, mundo");
}

// Función flecha
let saludar = () => {
    console.log("Hola, mundo");
}

saludar(); // Llama a la función saludar
```

Esto significa que al llamar a la función `saludar`, se mostrará el mensaje "Hola, mundo" en la consola.

cosas a tener en cuenta:

- Las funciones flecha se definen con la sintaxis `() => {}`.
  
#### Recomendaciones

- [Explicación arrow function](https://www.youtube.com/watch?v=HVEkbCZAuqA)