### Tipos de for

Hasta ahora hemos visto el `for` y el `for...in`, pero hay otro tipo de for que es muy útil, el `for...of`. El `for...of` se utiliza para recorrer arreglos y otros objetos iterables, como cadenas de texto, mapas, conjuntos, y más. Es muy útil cuando se necesita recorrer los elementos de un arreglo y realizar operaciones con cada elemento.

```javascript
let colores = ["rojo", "verde", "azul"];

for (let color of colores) {
    console.log(color); // Imprimir cada elemento del arreglo
}
```

Esto significa que al recorrer el arreglo `colores` con un bucle `for...of`, se imprimirá cada elemento del arreglo en la consola. En este caso, se imprimirán los valores `"rojo"`, `"verde"` y `"azul"`. Podemos notar que no necesitamos un indice para acceder a los elementos, sino que accedemos directamente al elemento. ¿Entonces cuando usar `for` y cuando usar `for...of`? Pues si necesitas el indice, usa `for`, si no necesitas el indice, usa `for...of`.

### Retos

Vamos a unos retos matematicos con javascript que intente combinar todo lo que hemos visto hasta ahora sobre javascript que es variables, condicionales, bucles, funciones, arreglos y objetos. Tener una buena logica es muy importante en la programación, y estos retos son para que vayas adquiriendo esa logica.
> Nota: revisar [Math.random()](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Global_Objects/Math/random), esto con el fin de que puedas generar números aleatorios, entonces como trabajamos con números y arreglos, podemos crear un arreglo y llenarlo con números aleatorios para realizar las pruebas.

- Realizar un programa que calcule el area de un cuadrado.
- Realizar un programa que calcule el area de un rectangulo.
- Realizar un programa que calcule el area de un triangulo.
- Realizar un programa que calcule el area de un circulo.
- Realizar un programa que calcule el area de una figura dada.
- Realizar un programa que dado un arreglo de numeros, devuelva el valor maximo, el valor minimo y el promedio.
- Realizar un programa que dado un arreglo de numeros, almacenar en un objeto la cantidad de numeros pares, la cantidad de numeros impares y la cantidad de ceros.