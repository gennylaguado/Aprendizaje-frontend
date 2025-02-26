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

##### Recomendaciones

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

##### Recomendaciones

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

##### Recomendaciones

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