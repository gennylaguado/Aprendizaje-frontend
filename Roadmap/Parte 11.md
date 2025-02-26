## Arrays / Arreglos

Entramos a uno de los tipos de datos más usados en muchos lenguajes de programación, los arreglos. Los arreglos se utilizan para almacenar múltiples valores en una sola variable. En JavaScript, los arreglos se definen con corchetes `[]` y los valores se separan por comas `,`.

```javascript
let colores = ["rojo", "verde", "azul"];

console.log(colores); // Imprimir el arreglo completo
```

Esto significa que el arreglo `colores` contiene los valores `"rojo"`, `"verde"` y `"azul"`. Al imprimir el arreglo completo, se mostrarán los valores en la consola.

cosas a tener en cuenta:

- Los arreglos se definen con corchetes `[]`.
- Los valores del arreglo se separan por comas `,`.
- Los valores del arreglo pueden ser números, cadenas de texto, booleanos, objetos, arreglos, y más.
- Los valores del arreglo se pueden acceder por posición, es decir, por índice.
- Los índices de los arreglos empiezan en 0, es decir, el primer elemento tiene índice 0, el segundo elemento tiene índice 1, y así sucesivamente.

#### Acceder a elementos

Se utiliza para acceder a un elemento específico de un arreglo por posición.

```javascript
let colores = ["rojo", "verde", "azul"];

console.log(colores[0]); // Acceder al primer elemento del arreglo

console.log(colores[1]); // Acceder al segundo elemento del arreglo

console.log(colores[2]); // Acceder al tercer elemento del arreglo
```

Esto significa que al acceder al elemento `colores[0]`, se mostrará el valor `"rojo"` en la consola, al acceder al elemento `colores[1]`, se mostrará el valor `"verde"`, y al acceder al elemento `colores[2]`, se mostrará el valor `"azul"`. Si notas, es un número lo que va dentro para el indice, entonces si quisieras recorrer (pasar por todos los elementos) ya sea para primir o quizás para hacer una operación como sumarle 1 a cada elemento, se puede hacer con un bucle (for, while, do-while).

#### Modificar elementos

Se utiliza para modificar un elemento específico de un arreglo por posición. Esto es normal en la programación, ya que a veces se necesita cambiar un valor específico de un arreglo o puede ser que se necesite cambiar un valor en un arreglo en función de una condición.

```javascript
let colores = ["rojo", "verde", "azul"];

console.log(colores); // Imprimir el arreglo completo

colores[1] = "amarillo"; // Modificar el segundo elemento del arreglo

console.log(colores); // Imprimir el arreglo completo
```

Esto significa que al modificar el elemento `colores[1]` con el valor `"amarillo"`, se cambiará el valor del segundo elemento del arreglo, y al imprimir el arreglo completo, se mostrará el nuevo valor en la consola. Entonces notaremos que en el primer console debemos ver el arreglo con los valores `"rojo"`, `"verde"`, `"azul"`, y en el segundo console debemos ver el arreglo con los valores `"rojo"`, `"amarillo"`, `"azul"`.

#### Longitud de un arreglo

Se utiliza para obtener la cantidad de elementos de un arreglo. Podemos preguntarnos para que sirve esto, y la respuesta es que a veces se necesita saber cuántos elementos tiene un arreglo para realizar operaciones, como recorrer el arreglo, sumar los elementos, encontrar el valor máximo, y más.

```javascript
let colores = ["rojo", "verde", "azul"];

console.log(colores.length); // Obtener la longitud del arreglo = 3
```

Esto significa que al obtener la longitud del arreglo `colores`, se mostrará la cantidad de elementos del arreglo en la consola. En este caso, el arreglo `colores` tiene 3 elementos, por lo que la longitud del arreglo es 3.

#### Recorrer un arreglo

Se utiliza para recorrer todos los elementos de un arreglo y realizar operaciones con cada elemento. Esto es muy útil cuando se necesita realizar una operación con cada elemento del arreglo, como imprimirlos, sumarlos, encontrar el valor máximo, y más.

```javascript
let colores = ["rojo", "verde", "azul"];

for (let i = 0; i < colores.length; i++) {
    console.log(colores[i]); // Imprimir cada elemento del arreglo
}
```

Esto significa que al recorrer el arreglo `colores` con un bucle `for`, se imprimirá cada elemento del arreglo en la consola. En este caso, se imprimirán los valores `"rojo"`, `"verde"` y `"azul"`.

cosas a tener en cuenta:

- Se utiliza un bucle `for` para recorrer el arreglo.
- La variable `i` se utiliza como índice para acceder a cada elemento del arreglo.
- La condición `i < colores.length` se utiliza para determinar cuántas veces se ejecuta el bucle.
- La expresión `colores[i]` se utiliza para acceder a cada elemento del arreglo por posición.
- Se puede utilizar el bucle `for` para realizar operaciones con cada elemento del arreglo, como imprimirlos, sumarlos, encontrar el valor máximo, y más.

Otro ejemplo de recorrer un arreglo, pero en este caso, se quiere sumar todos los elementos del arreglo para obtener el total, digamos puede ser un arreglo que simula almacenar los precios de los productos de alguna lista de compra y se quiere obtener el total de la compra.

```javascript
let precios = [100, 200, 300];

let total = 0; // Inicializar el total en 0 porque se va a sumar y se necesita un valor inicial.

for (let i = 0; i < precios.length; i++) {
    total += precios[i]; // Sumar cada elemento del arreglo al total
}

console.log(total); // Imprimir el total de la compra
```

Esto significa que al recorrer el arreglo `precios` con un bucle `for`, se sumarán todos los elementos del arreglo para obtener el total de la compra, y se mostrará el total en la consola. En este caso, el total de la compra es 600, ya que se sumaron los valores 100, 200 y 300. Esto funciona en un total de 3 ciclos, en el primer ciclo el total es 0 y se le suma el primer elemento del arreglo que es 100, teniendo un total de 100, pero todavia falta 2 ciclos más, en el segundo ciclo la variable total es 100 y se le suma el segundo elemento del arreglo que es 200, teniendo un total de 300, pero todavia falta 1 ciclo más, en el tercer ciclo el total es 300 y se le suma el tercer elemento del arreglo que es 300, teniendo un total de 600.

### Retos

- Realizar un programa que reciba un arreglo de números y devuelva la suma de todos los elementos.
- Realizar un programa que reciba un arreglo de números y devuelva el promedio de todos los elementos.
- Realizar un programa que reciba un arreglo de números y devuelva el valor máximo.
- Realizar un programa que reciba un arreglo de números y devuelva el valor mínimo.
- Realizar un programa que reciba un arreglo de números y devuelva un nuevo arreglo con los elementos al cuadrado.
- Realizar un programa que reciba un arreglo de números y devuelva un nuevo arreglo con los elementos al cubo.
- Realizar un programa que reciba un arreglo de números y devuelva un nuevo arreglo con los elementos al cuadrado si son pares y al cubo si son impares.
- Realizar un programa que reciba un arreglo de números y devuelva un nuevo arreglo con los elementos ordenados de menor a mayor.
- Realizar un programa que reciba un arreglo de números y devuelva un nuevo arreglo con los elementos ordenados de mayor a menor.
- Realizar un programa que reciba un arreglo de números y devuelva un nuevo arreglo con los elementos únicos, es decir, sin elementos repetidos.
- Realizar un programa que reciba un arreglo de números y devuelva un nuevo arreglo con los elementos que se repiten.
- Realizar un programa que reciba un arreglo de números y devuelva un nuevo arreglo con los elementos que no se repiten.