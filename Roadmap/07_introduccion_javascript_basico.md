# JavaScript

![Descripción de la imagen](https://raw.githubusercontent.com/cat-milk/Anime-Girls-Holding-Programming-Books/master/Javascript/Maya_Yamato_Holding_Javascript_For_Absolute_Beginners.png)

> 💡 Nota: He agregado muchos enlaces a videos con el fin de encontrar una explicación más visual. A veces, los videos muestran los conceptos en otros lenguajes de programación, ¡pero eso es lo encantador de la programación! 🌐 Los conceptos son casi siempre los mismos, y solo cambia la sintaxis.

---

## ✨ Introducción a JavaScript

JavaScript es un lenguaje de programación que se utiliza para crear páginas web interactivas. Es un lenguaje de programación de alto nivel, interpretado y orientado a objetos. JavaScript se ejecuta en el navegador web del usuario, lo que permite interactuar con los elementos de la página, realizar cálculos, enviar y recibir datos, y mucho más.

JavaScript es un lenguaje de programación que se utiliza para crear páginas web interactivas 🖱️💻. Es de alto nivel, interpretado y orientado a objetos. Se ejecuta directamente en el navegador del usuario, lo que permite:

- Interactuar con los elementos de una página
- Realizar cálculos
- Enviar y recibir datos
- ¡Y mucho más!

---

## 🧠 Diferencias clave

- **¿Lenguaje de programación vs lenguaje de marcado?**
Un lenguaje de programación se usa para dar instrucciones que la computadora puede ejecutar. Permite tomar decisiones, hacer cálculos y controlar el flujo del programa.
Un lenguaje de marcado (como HTML) se usa para estructurar contenido. Define cómo se ven los elementos, pero no se ejecuta como tal.

- **¿Qué es un lenguaje de alto nivel?**
Es un lenguaje que se parece mucho al lenguaje humano. Es fácil de leer y escribir. Ejemplos: Python, JavaScript, TypeScript, Java...

- **¿Qué significa que sea interpretado?**
Significa que el código se ejecuta línea por línea, sin necesidad de compilarlo. Ideal para escribir y probar directamente en el navegador.

---

## 🚀 ¿Por qué aprender JavaScript?

Porque es uno de los lenguajes más populares del mundo 🌍. Se puede usar para crear:

- Aplicaciones web
- Juegos 🎮
- Aplicaciones móviles 📱
- Backends con Node.js
- Y más...

💡 Esencial para cualquier desarrollador web que quiera crear páginas dinámicas e interactivas.

### 🔗 Recomendaciones

- [¿Qué es la programación](https://www.youtube.com/watch?v=a7eznAouNak&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=1)
- [JavaScript en 5 minutos](https://youtu.be/FuCiNVP88pc?si=y3s5ILbUW8uf2bDq)

---

## 🛠️ Uso de la consola del navegador

La consola del navegador es una herramienta muy útil para interactuar con código JavaScript directamente desde la página web.

- **¿Cómo abrirla?**
Presionar F12 o hacer clic derecho → "Inspeccionar" → pestaña "Consola".

- **¿Para qué sirve?**
  - Probar código rápido
  - Ver mensajes (console.log)
  - Depurar errores
  - Inspeccionar variables

- ¿Qué es depurar código?: Depurar código es el proceso de identificar y corregir errores en un programa. Podemos decir que depurar es como ir buscando errores en el código mientras se prueba, y corregirlos para que el programa funcione correctamente.

Ejemplo:

```javascript
console.log("Hola, mundo!"); // Muestra "Hola, mundo!" en la consola
```

📝 También podemos escribir el código en un archivo .js y enlazarlo en tu HTML:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi página web</title>
    <script src="mi-script.js"></script> <!-- Enlazamos el archivo JavaScript -->
</head>
<body>
    <h1>Hola, mundo!</h1>
    <!-- Otro modo sin crear un archivo .js -->
    <script>
        console.log("Hola desde el HTML!"); // Muestra "Hola desde el HTML!" en la consola
    </script>
</body>
</html>
```

---

## 📐 Sintaxis básica

La sintaxis es como la gramática de un lenguaje: define cómo escribir instrucciones que la computadora pueda entender correctamente. Es decir, el texto que se escribe en un lenguaje de programación debe seguir ciertas reglas para que la computadora pueda entenderlo y ejecutarlo correctamente. Así como en un idioma se utilizan reglas gramaticales para formar oraciones coherentes y entendibles para otros, en un lenguaje de programación se utilizan reglas de sintaxis para formar instrucciones que la computadora pueda interpretar y ejecutar.
Algunos conceptos básicos de la sintaxis de JavaScript son:

### 💬 Comentarios

Sirven para explicar el código. Es decir, son anotaciones que se agregan al código para aclarar su funcionamiento o propósito. Los comentarios no afectan la ejecución del programa y son útiles para que otros programadores (o usted mismo en el futuro) entiendan mejor el código.

```javascript
// Este es un comentario de una línea, es decir, solo ocupa una línea, si se quiere escribir más líneas, se debe usar // en cada línea o usar el siguiente formato

/*
Este es un comentario
de varias líneas
*/
```

### 📦 Variables

Las variables se utilizan para almacenar valores en un programa. En JavaScript, se pueden declarar variables con la palabra clave `let`, `const`, o `var`, seguida del nombre de la variable y el valor que se le asigna.

```javascript
let nombre = "Juan";
const edad = 25;
var altura = 1.75;
```

📌 Cosas importantes:

- `let`: se utiliza para declarar variables que pueden cambiar de valor. Es decir, se pueden reasignar o cambiar su valor en otro momento del programa.
- `const`: se utiliza para declarar variables que no pueden cambiar de valor. Es decir, una vez que se asigna un valor a una variable constante, no se puede cambiar.
- `var`: se utilizaba en versiones antiguas de JavaScript para declarar variables, pero en la actualidad se recomienda utilizar `let` y `const` en su lugar.
- Estas palabras claves deben ser en minúsculas, es decir, `let`, `const`, `var`, no se pueden escribir en mayúsculas, por ejemplo, `Let`, `Const`, `VAR`.
- Los nombre de las variables suelen ser en minúsculas, y si son compuestas, se recomienda separar con guiones bajos `_` o con notación camelCase. No pueden empezar con números, ni contener espacios, ni caracteres especiales, ni palabras reservadas (por ejemplo, let, const, var, function, etc.).
- Las variables deben ser unicas, es decir, no se pueden declarar dos variables con el mismo nombre en el mismo ámbito o alcance (esto se verá más adelante).

🐫 Convención común: camelCase para nombrarlas → nombreCompleto.

#### 🔗 Recomendación

- [¿Qué es una variable?](https://www.youtube.com/watch?v=kZfuJvkdcHU&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=2)

### 📊 Tipos de datos

Los tipos de datos en JavaScript se utilizan para representar diferentes tipos de valores, como números, cadenas de texto, booleanos, objetos, arreglos, y más. Esto con el fin de que la computadora pueda entender y manipular esos valores de manera adecuada. Cada tipo de dato tiene sus propias características y se utiliza en diferentes situaciones. Por ejemplo en la vida real podemos tener diferentes tipos de datos que al leerlos podemos saber que se puede hacer con ellos o que representan. Por ejemplo, un número entero se puede sumar o restar, mientras que una cadena de texto se puede concatenar o dividir, entonces digamos una placa de un auto, podemos decir que es un número entero, pero también puede ser una cadena de texto, ya que puede contener letras y números. Entonces, al leer la placa podemos saber que se puede hacer con ella o que representa.

Algunos tipos de datos básicos en JavaScript son:

```javascript
let numero = 10; // Número
let decimal = 3.14; // Decimal
let texto = "Hola"; // Cadena
let esVerdadero = true; // Booleano
let persona = {nombre: "Juan", edad: 25}; // Objeto
let colores = ["rojo", "verde", "azul"]; // Arreglo
```

📌 Notas:

- Números: pueden ser enteros o decimales.
- Cadenas: comillas simples `'` o dobles `"`, es decir, `"Hola"` o `'Hola'`.
- Booleanos: `true` o `false`.
- Objetos: Se utilizan para almacenar múltiples valores en una sola variable. Se definen con llaves `{}` y se acceden por clave, es decir, `persona.nombre` o `persona.edad`. Por ejemplo, al presentarnos podemos decir que somos una persona, y podemos tener diferentes atributos como nombre, edad, altura, peso, etc. Entonces, al leer la presentación podemos saber que somos una persona y que tenemos diferentes atributos.
- Arreglos: Se utilizan para almacenar múltiples valores en una sola variable, y se acceden por índice. Es diferente a un objeto, ya que en un objeto se accede por clave, mientras que en un arreglo se accede por índice. Por ejemplo, al decir que tenemos una lista de colores, podemos decir que tenemos una lista de colores y podemos tener diferentes colores como rojo, verde, azul, etc. Entonces, al leer la lista de colores podemos saber que tenemos una lista de colores y que tenemos diferentes colores. Se definen con corchetes `[]` y se acceden por posición, es decir, `colores[0]` devuelve el primer color, `colores[1]` devuelve el segundo color, y así sucesivamente.

💡 JavaScript es dinámico y débilmente tipado: puedes cambiar el tipo de valor de una variable sin error.

#### 🔗 Recomendaciones

- [Entender un array o arreglo, el de los []](https://www.youtube.com/watch?v=k24J92Hod50)
- [Otra explicación de los array o arreglos](https://www.youtube.com/watch?v=_FsRvYZNbnc&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=7)