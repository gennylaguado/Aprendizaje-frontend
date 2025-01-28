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