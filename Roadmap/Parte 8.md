### Operadores básicos

Los operadores en JavaScript se utilizan para realizar operaciones matemáticas, comparaciones, asignaciones, y más. Algunos operadores básicos en JavaScript son:

#### Operadores aritméticos

Se utilizan para realizar operaciones matemáticas, como suma, resta, multiplicación, división, y más.

```javascript
let suma = 10 + 5; // Suma
let resta = 10 - 5; // Resta
let multiplicacion = 10 * 5; // Multiplicación
let division = 10 / 5; // División
let modulo = 10 % 5; // Módulo
```

cosas a tener en cuenta:

- El operador de suma `+` se puede utilizar para concatenar cadenas de texto.
- El operador de módulo `%` devuelve el resto/residuo de la división entre dos números.
- Los operadores aritméticos siguen las reglas de precedencia matemática, es decir, se evalúan en un orden específico. Por ejemplo, la multiplicación y la división tienen mayor precedencia que la suma y la resta.
- Se pueden utilizar paréntesis `()` para cambiar el orden de evaluación de los operadores.
- Los operadores aritméticos se pueden combinar con variables y valores para realizar cálculos.
- Los operadores aritméticos se pueden utilizar con números enteros y decimales.
- Los operadores aritmeticos se pueden utilizar para varios números, no solo dos, por ejemplo, `10 + 5 - 3`.

#### Operadores de comparación

Se utilizan para comparar dos valores y devolver un valor booleano `true` o `false`.

```javascript
let esIgual = 10 == 5; // Igual a (compara el valor) ¿10 es igual a 5?
let esDiferente = 10 != 5; // Diferente de (compara el valor) ¿10 es diferente de 5?
let esMayor = 10 > 5; // Mayor que (compara el valor) ¿10 es mayor que 5?
let esMenor = 10 < 5; // Menor que (compara el valor) ¿10 es menor que 5?
let esMayorIgual = 10 >= 5; // Mayor o igual que (compara el valor) ¿10 es mayor o igual que 5?
let esMenorIgual = 10 <= 5; // Menor o igual que (compara el valor) ¿10 es menor o igual que 5?

// texto
let esIgualTexto = "hola" == "mundo"; // ¿"hola" es igual a "mundo"?

// booleanos
let esIgualBooleano = true == false; // ¿true es igual a false?
```

cosas a tener en cuenta:

- El operador de igualdad `==` compara los valores de dos variables, pero no compara el tipo de dato. Por ejemplo, `10 == "10"` devuelve `true`.
- El operador de desigualdad `!=` devuelve `true` si los valores de dos variables son diferentes.
- Se pueden utilizar los operadores de comparación con números, cadenas de texto, booleanos, y más.

#### Operadores lógicos

Se utilizan para combinar dos o más expresiones lógicas y devolver un valor booleano `true` o `false`.

```javascript
let menor = 10 < 5 && 5 < 3; // Y lógico (AND) ¿10 es menor que 5 y 5 es menor que 3?
let mayor = 10 > 5 || 5 < 3; // O lógico (OR) ¿10 es mayor que 5 o 5 es menor que 3?
let y = true && false; // Y lógico (AND) ¿true y false?
let o = true || false; // O lógico (OR) ¿true o false?
let no = !true; // Negación lógica (NOT) ¿no true?
```

cosas a tener en cuenta:

- El operador `&&` devuelve `true` si ambas expresiones son verdaderas.
- El operador `||` devuelve `true` si al menos una de las expresiones es verdadera.
- El operador `!` devuelve `true` si la expresión es falsa y `false` si la expresión es verdadera. Es decir, invierte el valor de la expresión.
- Los operadores lógicos se pueden combinar con operadores de comparación para realizar operaciones más complejas. Por ejemplo, `10 > 5 && 5 < 3` devuelve `false`, porque la primera expresión es verdadera y la segunda es falsa, entonces como ambas deben ser verdaderas para que el `&&` devuelva `true`, entonces devuelve `false`.

#### Operadores de asignación

Se utilizan para asignar un valor a una variable.

```javascript
let x = 10; // Asignación simple
let y = 5;
y = y + 3; // Asignación de suma (y = y + 3)
y += 3; // Asignación de suma (y = y + 3) Forma abreviada
y = y - 3; // Asignación de resta (y = y - 3)
y -= 3; // Asignación de resta (y = y - 3) Forma abreviada
y *= 3; // Asignación de multiplicación (y = y * 3)
y /= 3; // Asignación de división (y = y / 3)
y %= 3; // Asignación de módulo (y = y % 3)
y = y + 1; // Asignación de sumar uno
y++; // Asignación de sumar uno

```

cosas a tener en cuenta:

- Los operadores de asignación se pueden combinar con operadores aritméticos para realizar operaciones matemáticas y asignar el resultado a una variable.

##### Recomendaciones

- [¿Qué son los condicionales?](https://www.youtube.com/watch?v=RaWfeVgkWbE&list=PLPmRzmMDGerWEzjT0Vqy8D-IixKMY_6N6&index=3)