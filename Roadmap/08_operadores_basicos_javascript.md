# 🧮 Operadores Básicos en JavaScript

En JavaScript, los **operadores** son símbolos especiales que permiten realizar tareas como operaciones matemáticas, comparaciones, asignaciones y más.

---

## ➕ Operadores Aritméticos

Se utilizan para hacer operaciones matemáticas como suma, resta, multiplicación, etc.

```javascript
let suma = 10 + 5;           // Suma
let resta = 10 - 5;          // Resta
let multiplicacion = 10 * 5; // Multiplicación
let division = 10 / 5;       // División
let modulo = 10 % 5;         // Módulo (resto de la división), por ejemplo, 10 % 3 = 1 que es diferente a decir 10 / 3 = 3.33..., el 1 es el resto de la división y 3 es el cociente.
```

✅ Cosas a tener en cuenta:

- El operador `+` también sirve para concatenar cadenas de texto. Concatenar significa unir dos o más cadenas de texto. Por ejemplo, `"Hola" + "-" + "Mundo"` devuelve `"Hola-Mundo"`.
- El operador `%` devuelve el residuo de una división.
- Los operadores siguen la jerarquía matemática: multiplicación y división primero, luego suma y resta.
- Puedes usar paréntesis () para controlar el orden de evaluación. Así como en matemáticas, puedes usar paréntesis para cambiar el orden de evaluación de los operadores. Por ejemplo, `10 + 5 * 2` devuelve `20`, pero `(10 + 5) * 2` devuelve `30`.
- Funcionan con números enteros y decimales.
- Podemos encadenar operaciones. Es decir, se pueden utilizar para varios números, no solo dos.

    ```javascript
    let resultado = 10 + 5 - 3;
    resultado = resultado * 2; // resultado = 10 + 5 - 3 * 2
    resultado = (10 + 5 - 3) * 2; // resultado = 10 + 5 - 3 * 2
    ```

Quiero que notemos algo muy especial en la línea 2, y es que en la operación se está utilizando una variable `resultado`, y multiplicando por 2; a lo que quiero ir es que los operadores o generalmente en programación no siempre se van a utilizar directamente números o letras, sino que es muy normal es utilizar una variable y aplicarle una operación, y eso es lo que se está haciendo en la línea 2. Tambien hacer incapie en que cada vez que se llama una variable, el computador lo que hace es ver y decir "ah, esto es una variable, no un valor directamente, entonces voy a ir a la caja magica de variables y ver que hay dentro de ella, y lo que hay dentro de ella traerlo y ponerlo en la posición donde se está utilizando la variable". Entonces, si en la línea 2 se llama a la variable `resultado`, el computador va a la caja mágica de variables y ve primero si existe esa variable, si es así, ve que valor hay dentro de ella, y lo trae y lo pone en la posición donde se está utilizando la variable.

## 🔍 Operadores de Comparación

Se utilizan para comparar valores y devuelven true o false dependiendo del resultado. Es decir, similar a como nuestra mente compara cosas y se pregunta si cumple o no cumple con una condición. Ejemplo, supongamos que tenemos una manzana verde y una pera, y nos preguntamos si la manzana verde es igual a la pera, entonces nuestra mente compara las dos cosas y dice "no, no son iguales", entonces devuelve `false`. O si tenemos una manzana verde y una manzana roja, y nos preguntamos si son iguales, entonces nuestra mente compara las dos cosas y dice "sí, son iguales", entonces devuelve `true`; pero podemos ir más allá y comparar si el color de la manzana verde es igual al color de la pera, entonces nuestra mente compara los dos colores y dice "sí, son iguales", entonces devuelve `true`. Entonces, los operadores de comparación son similares a como nuestra mente compara cosas y se pregunta si cumple o no cumple con una condición.

El computador realmente no es que guarde la comparación, sino que realmente en el momento que llega a la comparación, lo que hace es resolverla y devolver el resultado, y en caso de que esa comparación se haga en una asignación de valor a una variable, entonces el computador dice ah, resolví la comparación y devolví el resultado, pero veo que hay una asignación acá, entonces tomo el resultado y lo guardo en la variable.

```javascript
let esIgual = 10 == 5;           // ¿10 es igual a 5? false
let esDiferente = 10 != 5;       // ¿10 es diferente de 5? true
let esMayor = 10 > 5;            // ¿10 es mayor que 5? true
let esMenor = 10 < 5;            // ¿10 es menor que 5? false
let esMayorIgual = 10 >= 5;      // ¿10 es mayor o igual que 5? true
let esMenorIgual = 10 <= 5;      // ¿10 es menor o igual que 5? false

// Comparación de texto
let texto = "hola" == "mundo";   // ¿"hola" es igual a "mundo"? false
let texto2 = "hola" == "hola";   // ¿"hola" es igual a "hola"? true
let texto3 = "hola" == "Hola";   // ¿"hola" es igual a "Hola"? false. Notar que la "H" es mayúscula y la "h" es minúscula, entonces no son iguales.

// Comparación de booleanos
let bool = true == false;        // ¿true es igual a false? false. Nos podemos preguntar acá que sentido tiene comparar un booleano con otro booleano, pero podemos tomar de que esos booleanos fueron resultados de otras comparaciones, entonces podemos decir que es válido comparar un booleano con otro booleano, ya que esos booleanos pueden ser el resultado de otras comparaciones.
let bool = (5 > 3) == (10 < 5); // Podemos usar esto como ejemplo para escalar el anterior.

// ¿Podemos hacer más de una comparación en una misma línea?
// Supongamos que queremos comparar caracteristicas de un objeto vehiculo, y queremos saber si es una moto o un auto
let vehiculo = {
    maxPasajeros: 2,
    ruedas: 2,
    color: "rojo",
};

// forma larga

// comparar pasajeros
let esMotoPorPasajeros = vehiculo.pasajeros == 2; // ¿es una moto? podriamos decir que sí, pero no es del todo cierto, ya que hay autos que tienen para solo 2 pasajeros, entonces debemos agregar más comparaciones
// comparar ruedas
let esMotoPorRuedas = vehiculo.ruedas == 2;

if (esMotoPorPasajeros && esMotoPorRuedas) {
    console.log("Es una moto");
} else {
    console.log("No es una moto");
}

// forma corta
let esMoto = vehiculo.pasajeros == 2 && vehiculo.ruedas == 2; // Notemos que tenemos 2 comparaciones de igualdad unidas por el operador lógico && (siguiente sección se explica), que en lenguaje natural es "y" o "and", que en nuestra mente cuando usamos dicha letra, es algo que en automatico nos hace pensar en que ambas condiciones deben ser verdaderas para que la comparación sea verdadera, por ejemplo, "si tengo dinero y tengo tiempo, entonces puedo ir al cine", pero si no tengo dinero o no tengo tiempo, entonces no puedo ir al cine. Entonces podemos darnos cuenta con que una sola condición no se cumpla en el "y" ya se convierte todo el resultado automaticamente en false.
```

cosas a tener en cuenta:

- El operador de igualdad `==` (dos igual) compara los valores de dos variables, pero no compara el tipo de dato. Por ejemplo, `10 == "10"` devuelve `true`, a pesar de que uno es un número y el otro es una cadena de texto. Si queremos comparar el tipo de dato también, debemos usar el operador `===` (tres igual), que compara tanto el valor como el tipo de dato. Por ejemplo, `10 === "10"` devuelve `false`, porque uno es un número y el otro es una cadena de texto.
- El operador de desigualdad `!=` devuelve `true` si los valores de dos variables son diferentes.
- Se pueden utilizar los operadores de comparación con números, cadenas de texto, booleanos, y más.

---

## 🤔 Operadores Lógicos

Sirven para combinar/unir condiciones y devolver un valor booleano (`true` o `false`).

```javascript
let resultado1 = 10 < 5 && 5 < 3;   // AND lógico
let resultado2 = 10 > 5 || 5 < 3;   // OR lógico
let resultado3 = true && false;    // AND
let resultado4 = true || false;    // OR
let resultado5 = !true;            // NOT
```

Para esto podemos buscar en internet "tabla de verdad" y ver como funcionan los operadores lógicos, pero en resumen:

- `&&` (AND): devuelve true solo si ambas condiciones son verdaderas. Ejemplo en nuestra mente cuando estamos en una conversación y decimos "si tengo dinero y tengo tiempo, entonces puedo ir al cine", pero si no tengo dinero o no tengo tiempo, entonces no puedo ir al cine. Es decir, si tenemos una condición entre un && y que es falsa, entonces el resultado final de todo eso es falso de golpe.
- `||` (OR): devuelve true si al menos una condición es verdadera. Ejemplo en nuestra mente cuando estamos en una conversación y decimos "voy al cine si mi novia o mi amigo me invitan", entonces si mi novia me invita, voy al cine, y si mi amigo me invita, voy al cine, pero si ninguno de los dos me invita, no voy al cine. Es decir, si tenemos una condición entre un || y que es falsa, entonces el resultado final de todo eso es verdadero de golpe.
- `!` (NOT): invierte el valor booleano.

## ✍️ Operadores de Asignación

Se usan para asignar valores a variables, y también permiten combinarse con los otros operadores para realizar operaciones y asignar el resultado a la variable.

```javascript
let x = 10;      // Asignación básica
let y = 5;

y = y + 3;       // Suma directa
y += 3;          // Suma abreviada
y -= 3;          // Resta abreviada
y *= 3;          // Multiplicación abreviada
y /= 3;          // División abreviada
y %= 3;          // Módulo abreviado

y = y + 1;       // Incremento clásico
y++;             // Incremento abreviado

z = 5 > 3; // Asignación de un valor booleano, es decir, cuando vayamos a usar a `z`, estariamos invocando un `true` o `false`, dependiendo de la comparación que se haya hecho.
```

## 🔗 Recomendaciones

- [¿Qué son los condicionales?](https://www.youtube.com/watch?v=RaWfeVgkWbE&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=3)
