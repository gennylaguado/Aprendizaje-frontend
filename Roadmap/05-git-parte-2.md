# 🌟 Más sobre Git

## Ver Cambios en Archivos 🧐

Comando principal:

```bash
git diff
```

Este comando te permite ver qué cambios has hecho en tus archivos desde el último commit.

📌 Detalles importantes:

- 🟩 Líneas en verde → Son las que se han agregado.
- 🟥 Líneas en rojo → Son las que se han eliminado.
- ⚪ Líneas en blanco → Son las que no han cambiado.
- 🔙 Para salir de la vista de cambios, presiona q.

📂 Opciones útiles:

- `git diff <archivo>` Muestra los cambios en un archivo específico.
- `git diff <commit1> <commit2>` Muestra las diferencias entre dos commits.
- `git diff --staged` Muestra los cambios que ya están en el Staging Area.

🎯 Reto:

- Modifica un archivo y usa `git diff`.
- Agrega los cambios al Staging Area y usa `git diff --staged`.
- Compara los cambios entre dos commits usando `git diff <commit1> <commit2>`.

## Deshacer Cambios 🔄

🚫 Comandos clave:

1. Descartar cambios en un archivo (volver al último commit)

    ```bash
    git checkout -- <archivo>
    ```

    ⚠️ Tener cuidado, ya que se perderán los cambios no guardados.

2. Sacar un archivo del Staging Area (pero sin perder los cambios)

    ```bash
    git reset HEAD <archivo>
    ```

3. Deshacer un commit (manteniendo los cambios en el directorio de trabajo)

    ```bash
    git reset --soft HEAD~1
    ```

    Esto elimina el último commit pero mantiene los cambios sin perderlos.

🎯 Reto:

- Modifica un archivo y agrégalo al Staging Area.
- Usa `git reset HEAD <archivo>` para sacarlo del Staging Area.
- Realiza un commit y luego usa `git reset --soft HEAD~1` para deshacerlo.

## Trabajando con Ramas 🌿

Las ramas en Git permiten trabajar en nuevas funcionalidades sin afectar la rama principal.

📌 Comandos clave:

- Ver las ramas existentes

    ```bash
    git branch
    ```

- Crear una nueva rama

    ```bash
    git branch <nombre_rama>
    ```

- Cambiar de rama

    ```bash
    git checkout <nombre_rama>
    ```

- Crear y cambiar a una rama en un solo paso

    ```bash
    git checkout -b <nombre_rama>
    ````

🎯 Reto:

- Crea una nueva rama.
- Cambia a la nueva rama y realiza un commit.
- Regresa a la rama main.

## Fusionar Ramas 🔀

Para unir los cambios de una rama en otra, usamos merge.

- Comando principal:

    ```bash
    git merge <nombre_rama>
    ```

    Si hay conflictos, Git te pedirá resolverlos manualmente antes de completar la fusión.

🎯 Reto:

- Crea una nueva rama y realiza cambios en un archivo.
- Regresa a main y fusiónala con `git merge <nombre_rama>`.
- Si hay conflictos, resuélvelos y completa la fusión.

## Clonar un Repositorio 🔗

Para copiar un repositorio remoto en tu máquina local, usa:

```bash
git clone <URL>
```

📌 Ejemplo:

```bash
git clone https://github.com/usuario/repositorio.git
```

🎯 Reto:

- Busca un repositorio público en GitHub.
- Clónalo en tu máquina y explora su estructura.