# 🌟 Introducción a CSS

CSS es el lenguaje que le da vida y estilo a nuestras páginas web. Si HTML es el esqueleto de un sitio, CSS es la ropa y los accesorios que lo hacen ver bien. En este apartado aprenderemos lo básico para empezar a personalizar nuestras interfaces.

## Lo primero: ¿Qué es CSS?

CSS **(Cascading Style Sheets)** es un lenguaje de estilos que nos permite modificar la apariencia de los elementos HTML. Con CSS podemos cambiar colores, fuentes, tamaños, posiciones y mucho más.

## 👉 Cómo enlazar CSS con HTML

Para aplicar estilos a nuestro HTML, podemos hacerlo de tres formas:

- **CSS en línea (inline)** Se escribe directamente dentro del atributo style de un elemento. Es poco recomendable porque hace que el código sea difícil de mantener.

    ```html
    <p style="color: red; font-size: 20px;">Hola, mundo!</p>
    ```

- **CSS interno** Se coloca dentro de una etiqueta `<style>` en el `<head>` del documento. Se usa cuando los estilos son específicos para una página en particular.

    ```html
    <style>
    p {
        color: blue;
    }
    </style>
    ```

- **CSS externo (la mejor práctica)** Se guarda en un archivo separado (styles.css) y se enlaza en el `<head>` del HTML con la etiqueta `<link>`.

```html
<link rel="stylesheet" href="styles.css">
```

## 🎭 Selectores básicos

Los selectores en CSS nos permiten apuntar a los elementos que queremos estilizar. Estos son los más comunes:

### 🔗 Selectores de elementos, clases e IDs

```css
/* Selector de elemento */
p {
  color: red;
}

/* Selector de clase */
.my-class {
  font-size: 20px;
}

/* Selector de ID */
#my-id {
  background-color: blue;
}
```

>**Nota:** Los selectores de clase (`.mi-clase`) son reutilizables en varios elementos, mientras que los IDs (`#mi-id`) deben ser únicos en cada página.

### Selectores combinados

Podemos combinar selectores para hacer reglas más específicas:

```css
/* Aplica estilo a los <p> dentro de un <div> */
div p {
  color: red;
}

/* Aplica estilo solo a <div> con la clase "my-class" */
div.my-class {
  font-size: 20px;
}

/* Aplica estilo solo a <p> con clase "my-class" dentro de un <div> */
div p.my-class {
  font-size: 20px;
}
```

>**Tip:** Para aplicar estilos solo a elementos que están directamente dentro de otro (sin otros elementos en medio), usamos `>`.

```css
div > p {
  color: green;
}
```

## 💡 Propiedades esenciales

Algunas propiedades básicas para empezar:

- Colores: `color`, `background-color`
- Tipografía: `font-size`, `font-family`, `line-height`
- Espaciado: `margin`, `padding`
- Bordes y sombras: `border`, `box-shadow`

[Lista de propiedades CSS](https://carontestudio.com/blog/listado-de-propiedades-css/)

## 🏰 Sistema de cajas (Box Model)

Cada elemento en CSS es una "caja" con cuatro áreas:

1. **Contenido** (el texto o imagen dentro del elemento)
2. **Padding** (espacio entre el contenido y el borde)
3. **Borde** (el límite del elemento)
4. **Margin** (espacio entre este elemento y otros elementos)

[Más detalles sobre el Box Model](https://www.w3schools.com/css/css_boxmodel.asp)

## 🛏️ Posicionamiento en CSS

CSS nos permite posicionar elementos de diferentes maneras:

- `static`: Posición por defecto (fluye con el documento).
- `relative`: Se mueve en base a su posición original.
- `absolute`: Se mueve en base a su contenedor más cercano con `position: relative`.
- `fixed`: Se mantiene fijo en la pantalla aunque hagamos scroll.

Ejemplo de `absolute` dentro de un `relative`:

```css
div {
  position: relative;
}

span {
  position: absolute;
  top: 10px;
  left: 20px;
}
```

## 🌟 Flexbox: Diseño flexible

Flexbox es una herramienta que facilita la distribución de elementos.

```css
.flex-container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

Algunas propiedades importantes:

- `justify-content`: Alinea elementos horizontalmente.
- `align-items`: Alinea elementos verticalmente.
- `flex-wrap`: Controla si los elementos se ajustan en una sola fila o se distribuyen en varias.

[Guía rápida de Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

## 🚀 Grid Layout: Diseños avanzados

Grid permite crear estructuras complejas con filas y columnas.

```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 10px;
}
```

Propiedades clave:

- `grid-template-columns`: Define el número y tamaño de las columnas.
- `grid-template-rows`: Define las filas.
- `gap`: Espacio entre elementos.

[Guía rápida de CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

## 🏆 Retos y Ejercicios

- Diseñar una página de currículum con estilos básicos.
- Crear una galería de imágenes con Flexbox (tres columnas).
