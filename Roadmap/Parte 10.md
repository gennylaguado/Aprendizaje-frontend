### Funciones

Las funciones en JavaScript se utilizan para encapsular un bloque de código y reutilizarlo en diferentes partes de un programa. Una función puede aceptar parámetros, realizar operaciones, y devolver un valor si es necesario.

Las funciones son muy importantes en un lengua de programación, ya que permiten dividir un programa en partes más pequeñas y fáciles de entender, reutilizar código, y realizar tareas específicas.

Algunos conceptos básicos de las funciones en JavaScript son:

#### Declaración de funciones

Se utiliza para definir una función y especificar los parámetros y el bloque de código que se ejecuta cuando se llama a la función.

```javascript
function saludar() {
    console.log("Hola, mundo");
}

saludar(); // Llama a la función saludar
```

Notemos la palabra reservada `function`, que se utiliza para declarar una función, y el nombre de la función `saludar`, que se utiliza para llamar a la función en otras partes del programa. El bloque de código de la función se encierra entre llaves `{}`. En este caso, el bloque de código de la función `saludar` es `console.log("Hola, mundo")`, que se ejecuta cuando se llama a la función `saludar`.

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

Ahora surge la pregunta, ¿Como hago para que la función `saludar` salude a una persona en específico? Para eso se utilizan los parámetros. Los parámetros se utilizan para pasar valores a una función y realizar operaciones con esos valores.

```javascript
function sumar(a, b) {
    let resultado = a + b;
    console.log(resultado);
}

sumar(5, 3); // Llama a la función sumar con los valores 5 y 3
sumar(10, 2); // Llama a la función sumar con los valores 10 y 2

// otro ejemplo con saludar

function saludar(nombre) {
    console.log("Hola, " + nombre);
}

saludar("Juan"); // Llama a la función saludar con el valor "Juan"
saludar("Genny"); // Llama a la función saludar con el valor "Genny"
```

Esto significa que al llamar a la función `sumar` con los valores 5 y 3, se mostrará el resultado de la suma en la consola, y al llamar a la función `sumar` con los valores 10 y 2, se mostrará el resultado de la suma en la consola.

cosas a tener en cuenta:

- Los parámetros se definen entre paréntesis `()` y se separan por comas `,`.
- Los parámetros se utilizan para pasar valores a una función y realizar operaciones con esos valores.
- Los parámetros se pueden utilizar en el bloque de código de la función como variables locales.
- Se pueden utilizar múltiples parámetros en una función para realizar operaciones más complejas.
- Los valores que se pasan a una función se llaman argumentos, es decir, se les dice parámetros cuando se define la función, y argumentos cuando se llama a la función. En los ejemplos, `a`, `b` y `nombre` son parámetros, y `5`, `3`, `10`, `2`, `Juan` y `Genny` son argumentos.

Acá se introdujo un nuevo termino que es "variables locales". Antes de esta sección, se habló de variables, que son como "cajas" (más adelante cambiará el concepto) que se utilizan para almacenar valores en un programa. Lo que sucedía es que esas variables se podían utilizar en cualquier parte del programa, es decir, eran "globales". Pero en este caso, las variables locales son variables que solo se pueden utilizar dentro de una función, es decir, solo son accesibles dentro de la función en la que se declaran. Esto es útil para evitar conflictos de nombres y mantener el código organizado. Por ejemplo, si se declara una variable `resultado` dentro de una función, solo se puede utilizar dentro de esa función, y no se puede acceder desde otras partes del programa. En la estructura `for` y `while` también se utilizan variables locales, ya que las variables de control solo se pueden utilizar dentro del bucle.

##### Recomendaciones

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

Esto es mucho lo que hablamos de imaginar como cajas dentro de cajas, es decir, si una caja está dentro de otra, la caja de afuera no puede acceder a la caja de adentro, pero la caja de adentro si puede acceder a la caja de afuera. En este caso, la variable `global` es una variable global, es decir, se puede acceder desde cualquier parte del programa, y la variable `local` es una variable local, es decir, solo se puede acceder desde la función en la que se declara.

El scope no solo se limita a funciones, realmente podemos imaginar como el alcance de una variable es dentro de un bloque de código, y podemos asumir los limites de ese bloque de código como las llaves `{}`.

#### Retorno de funciones (return)

Se utiliza para devolver un valor desde una función y utilizarlo en otras partes del programa. Por ejemplo, se puede utilizar una función para realizar un cálculo y devolver el resultado.

Anteriormente habiamos visto el ejemplo de la función `sumar`, que recibe numeros e imprime el valor, pero ahora vamos a modificarla para que devuelva el resultado en lugar de mostrarlo en la consola, ya que puede ser útil para utilizarlo en otras partes del programa y queremos que la función se encargue de realizar el calculo y devolver el resultado.

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

- La palabra reservada `return` se utiliza para devolver un valor desde una función.
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
  
##### Recomendaciones

- [Explicación arrow function](https://www.youtube.com/watch?v=HVEkbCZAuqA)

### Retos

- Realizar un programa que simule una calculadora con las operaciones básicas (suma, resta, multiplicación, división) y devuelva el resultado. Es decir, se recibe dos números y la operación a realizar, y se devuelve el resultado.
- Realizar un programa que reciba un número y devuelva si es par o impar.
- Realizar un programa que reciba un número y devuelva si es positivo, negativo o cero.
- Realizar un programa que reciba un número y devuelva su factorial.
- Realizar un programa que reciba un número y devuelva su tabla de multiplicar hasta el 10.
- Realizar un programa que reciba un número y devuelva su tabla de multiplicar hasta el un número específico.