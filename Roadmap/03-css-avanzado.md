# 🌟 CSS: Llevando los Estilos al Siguiente Nivel

## 🎯 Objetivo

Aprender cositas más avanzadas de CSS para crear diseños más dinámicos y atractivos.

## Pseudo-clases y Pseudo-elementos

Son selectores especiales que permiten aplicar estilos en ciertos estados de un elemento o insertar contenido antes o después de un elemento sin modificar el HTML.

**Pseudo-clases más comunes:**

- `:hover` Cambia el estilo cuando el usuario pasa el cursor sobre un elemento.
- `:active` Aplica estilos cuando el elemento está siendo presionado.
- `:focus` Estilos cuando un campo de formulario está enfocado.

```css
button:hover {
    background-color: red;
}
```

**Pseudo-elementos más utilizados:**

- `::before` y `::after` Permiten agregar contenido antes o después de un elemento.

```css
p::before {
    content: "Hola ";
    color: blue;
}
```

**Otros selectores útiles:**

- `p:first-child` Aplica estilos solo al primer `<p>` dentro de su contenedor.
- `p:nth-child(odd)` Selecciona los párrafos impares dentro del contenedor.
- `p:nth-child(2n)` Selecciona los párrafos en posiciones pares.

```css
p:first-child {
    color: red;
}

p:nth-child(odd) {
    color: green;
}
```

>**Tip**: Prueba estos selectores dentro de un contenedor con varios `<p>` para ver los efectos.

## Variables en CSS

Las variables en CSS permiten reutilizar valores como colores o tamaños de fuente de manera más eficiente. Se declaran en :root y se utilizan con var().

```css
:root {
    --main-color: #3498db;
}

p {
    color: var(--main-color);
}
```

## Animaciones y Transiciones

Las animaciones en CSS permiten crear efectos dinámicos sin necesidad de JavaScript.

- **Transiciones** para cambios suaves entre estados.

    ```css
    button {
        transition: background-color 0.5s;
    }

    button:hover {
        background-color: red;
    }
    ```

- **Animaciones** para secuencias más complejas con `@keyframes`.

```css
@keyframes example {
    0% { background-color: red; }
    100% { background-color: blue; }
}

div {
    animation: example 5s infinite;
}
```

## 📌 Guía de animaciones

### Responsive Design

El diseño responsivo permite que una web se vea bien en distintos tamaños de pantalla.

- **Media Queries** aplican estilos según el ancho de la pantalla.

    ```css
    @media screen and (max-width: 600px) {
        body {
            background-color: lightblue;
        }
    }
    ``

- **Unidades relativas** para mayor flexibilidad.

  - `%` Relativo al tamaño del contenedor padre.
  - `vw`, `vh` Relativo al ancho y alto de la ventana. `vw` es viewport width y `vh` es viewport height.
  - `em`, `rem` Relativo al tamaño de fuente. `em` es relativo al tamaño del elemento padre y `rem` al tamaño de fuente del root.

[Más sobre unidades](https://www.w3schools.com/css/css3_animations.asp)

## 🏆 Retos y Ejercicios

- Crear un menú de navegación con animaciones.
- Diseñar un portafolio responsive [Ejemplo](https://www.youtube.com/watch?v=YMZmJfCOp_s&ab_channel=divcode)
- Crear una galería de imágenes con transiciones (como que al pararse sobre una imagen, esa crece un poco, y al salir el mouse, la imagen vuelve a su tamaño original).
- Implementar un slider de logos animado [Ejemplo](https://www.youtube.com/watch?v=zf7r0l5PCwE&ab_channel=CodeGlitch)
- Crear un efecto de partículas en movimiento [Ejemplo](https://www.youtube.com/watch?v=fbn2aVaSb3E&ab_channel=SINERGIA)
- Agregar efecto de luz ambiental a una figura [Ejemplo](https://www.youtube.com/watch?v=nOdDtnHWaDo&ab_channel=OnlineTutorials)
- Implementar un efecto máquina de escribir (typewriter) [Ejemplo](https://www.youtube.com/shorts/fTOcWMD_5pk)
