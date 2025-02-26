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

### Comentarios

Los comentarios son texto que se utiliza para explicar el código y no se ejecutan. En JavaScript, los comentarios se pueden escribir de dos formas: con `//` para comentarios de una línea y con `/* */` para comentarios de varias líneas.

```javascript
// Este es un comentario de una línea

/*
Este es un comentario
de varias líneas
*/
```

### Variables

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

### Tipos de datos

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