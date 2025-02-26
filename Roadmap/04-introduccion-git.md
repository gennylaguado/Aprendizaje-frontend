# 🌟 Introducción a Git

Conceptos Básicos del Control de Versiones y Git

## 🧐 ¿Qué es el Control de Versiones y Git?

El control de versiones es una herramienta que nos permite llevar un historial de cambios en nuestros archivos, facilitando la colaboración con otras personas sin miedo a perder información.

**Git** es un sistema de control de versiones distribuido, lo que significa que cada persona que trabaja en el proyecto tiene una copia completa del historial de cambios. Es rápido, seguro y flexible.

## 🔧 Instalación de Git y Configuración Inicial

1. Descarga e instala Git desde [git-scm.com](https://git-scm.com/)

2. Configura Git en tu computadora con los siguientes comandos ejecutados en la terminal recomendada Bash:

    ```bash
    # Configura tu nombre
    git config --global user.name "Tu Nombre"

    # Configura tu correo
    git config --global user.email "tuemail@example.com"
    ```

    El nombre y el correo se usan para identificar quién hizo cada cambio en los commits.

3. Para verificar la configuración, usa:

    ```bash
    git config --list
    ```

## 📂 Trabajando con un Repositorio Local

1. 📌 Crear un Repositorio

    Para iniciar un nuevo proyecto con Git, usa el comando:

    ```bash
    git init
    ```

    Esto crea una carpeta oculta llamada .git, donde se almacenará el historial de cambios.

    📌 Para ver si se creó correctamente, usa:

    ```bash
    ls -a
    ```

2. 📌 Agregar Archivos al Staging Area

    Una vez que hayas modificado o creado archivos, debes agregarlos al Staging Area para prepararlos para un commit.

    ```bash
    git add <nombre_archivo>
    ```

    Si quieres agregar todos los archivos modificados de una sola vez:

    ```bash
    git add .
    ```

    Ejemplo:

    ```bash
    echo "Hola Git" > hola.txt
    git add hola.txt
    ```

    📌 Reto:

    - Crea dos archivos (`index.html` y `style.css`)
    - Usa git add para añadir solo uno al Staging Area.
    - Verifica con git status cuáles archivos están listos para el commit.

3. 📌 Guardar Cambios con un Commit

    Un commit es como un punto de guardado en el historial de cambios. Para hacer un commit usa:

    ```bash
    git commit -m "Descripción breve del cambio"
    ```

    📌 Ejemplo:

    ```bash
    git commit -m "Agregado el navbar al proyecto"
    ```

    El mensaje debe ser claro y explicar qué se cambió.

4. 📌 Ver el Historial de Cambios

    Para ver todos los commits realizados en el proyecto:

    ```bash
    git log
    ```

    💡 Opciones útiles:

    ```bash
    git log --oneline # Muestra un historial más compacto.

    git log --graph # Muestra un historial visual con ramas.
    ```

5. 📌 Ignorar Archivos con .gitignore

    A veces hay archivos que no queremos incluir en el repositorio (archivos temporales, credenciales, carpetas como node_modules). Para eso usamos el archivo .gitignore.

    - Creando un .gitignore

    ```bash
    echo "node_modules/" > .gitignore
    ```

    Esto le dice a Git que ignore la carpeta node_modules.

    📌 Practica:

    - Crea un archivo .gitignore
    - Agrega un archivo o carpeta a .gitignore
    - Usa git status para verificar que Git lo está ignorando correctamente.
