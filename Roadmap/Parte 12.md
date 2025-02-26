### Objetos

Entramos a otro tipo de dato muy importante en JavaScript, los objetos. Los objetos se utilizan para almacenar múltiples valores en una sola variable, pero a diferencia de los arreglos, los objetos almacenan los valores en pares de clave-valor. En JavaScript, los objetos se definen con llaves `{}` y los pares de clave-valor se separan por comas `,`. ¿Que podemos tener en el mundo real como un objeto clave-valor? Pues un ejemplo muy claro es un diccionario, donde la clave es la palabra y el valor es la definición de la palabra. Entonces imaginemos que el diccionario sea algo electronico donde nosotros le mandamos una palabra y nos devuelve la definición de la palabra.

```javascript
let persona = {
    nombre: "Juan",
    edad: 30,
    casado: false
};

console.log(persona); // Imprimir el objeto completo
```

Esto significa que el objeto `persona` contiene los pares de clave-valor `nombre: "Juan"`, `edad: 30` y `casado: false`. Al imprimir el objeto completo, se mostrarán los pares de clave-valor en la consola. Como puede notar, un objeto nos ayuda a organizar-agrupar información, en este caso, la información de una persona.

cosas a tener en cuenta:

- Los objetos se definen con llaves `{}`.
- Los pares de clave-valor se separan por comas `,`.
- Las claves se utilizan para acceder a los valores del objeto.
- Los valores del objeto pueden ser números, cadenas de texto, booleanos, objetos, arreglos, y más.

#### Acceder a propiedades

Se utiliza para acceder a un valor específico de un objeto por clave. Esto es muy útil cuando se necesita obtener un valor específico de un objeto para realizar operaciones, como imprimirlo, modificarlo, eliminarlo, y más.

```javascript
let persona = {
    nombre: "Juan",
    edad: 30,
    casado: false
};

console.log(persona.nombre); // Acceder a la propiedad nombre del objeto

console.log(persona.edad); // Acceder a la propiedad edad del objeto

console.log(persona.casado); // Acceder a la propiedad casado del objeto
```

Esto significa que al acceder a la propiedad `nombre` del objeto `persona`, se mostrará el valor `"Juan"` en la consola, al acceder a la propiedad `edad`, se mostrará el valor `30`, y al acceder a la propiedad `casado`, se mostrará el valor `false`.

#### Modificar propiedades

Se utiliza para modificar un valor específico de un objeto por clave. Esto es normal en la programación, ya que a veces se necesita cambiar un valor específico de un objeto o puede ser que se necesite cambiar un valor en un objeto en función de una condición.

```javascript
let persona = {
    nombre: "Juan",
    edad: 30,
    casado: false
};

console.log(persona); // Imprimir el objeto completo

persona.edad = 35; // Modificar la propiedad edad del objeto

console.log(persona); // Imprimir el objeto completo
```

Esto significa que al modificar la propiedad `edad` del objeto `persona` con el valor `35`, se cambiará el valor de la propiedad `edad` del objeto, y al imprimir el objeto completo, se mostrará el nuevo valor en la consola. Entonces notaremos que en el primer console debemos ver el objeto con las propiedades `nombre: "Juan"`, `edad: 30`, `casado: false`, y en el segundo console debemos ver el objeto con las propiedades `nombre: "Juan"`, `edad: 35`, `casado: false`.

#### Añadir propiedades

¿Que pasa si necesitamos añadir una propiedad a un objeto? Pues se puede hacer, y es muy útil cuando se necesita almacenar información adicional en un objeto o cuando se necesita añadir una propiedad en función de una condición.

```javascript
let persona = {
    nombre: "Juan",
    edad: 30,
    casado: false
};

console.log(persona); // Imprimir el objeto completo

persona.altura = 1.75; // Añadir la propiedad altura al objeto

console.log(persona); // Imprimir el objeto completo
```

Esto significa que al añadir la propiedad `altura` al objeto `persona` con el valor `1.75`, se añadirá la propiedad `altura` al objeto, y al imprimir el objeto completo, se mostrará la nueva propiedad en la consola. Entonces notaremos que en el primer console debemos ver el objeto con las propiedades `nombre: "Juan"`, `edad: 30`, `casado: false`, y en el segundo console debemos ver el objeto con las propiedades `nombre: "Juan"`, `edad: 30`, `casado: false`, `altura: 1.75`.

#### Eliminar propiedades

Se utiliza para eliminar una propiedad específica de un objeto por clave. Esto es muy útil cuando se necesita eliminar una propiedad de un objeto o cuando se necesita eliminar una propiedad en función de una condición. Después de eliminar una propiedad, ya no se puede acceder a ella.

```javascript
let persona = {
    nombre: "Juan",
    edad: 30,
    casado: false
};

console.log(persona); // Imprimir el objeto completo

delete persona.edad; // Eliminar la propiedad edad del objeto

console.log(persona); // Imprimir el objeto completo

console.log(persona.edad); // Error: la propiedad edad no está definida
```

Esto significa que al eliminar la propiedad `edad` del objeto `persona`, se eliminará la propiedad `edad` del objeto, y al imprimir el objeto completo, ya no se mostrará la propiedad `edad` en la consola. Entonces notaremos que en el primer console debemos ver el objeto con las propiedades `nombre: "Juan"`, `edad: 30`, `casado: false`, y en el segundo console debemos ver el objeto con las propiedades `nombre: "Juan"`, `casado: false`, y en el tercer console debemos ver un error que dice que la propiedad `edad` no está definida.

#### Recorrer un objeto

¿Podemos recorrer un objeto, y que sentido tiene recorrer un objeto? Pues si, se puede recorrer un objeto, y tiene sentido cuando se necesita realizar una operación con cada propiedad del objeto, como imprimirlas, modificarlas, eliminarlas, y más.

```javascript
let persona = {
    nombre: "Juan",
    edad: 30,
    casado: false
};

for (let propiedad in persona) {
    console.log(propiedad + ": " + persona[propiedad]); // Imprimir cada propiedad del objeto
}
```

> Nota: Observa el for, es un for...in, un for que no habiamos visto, pero es muy útil para recorrer objetos, su funcionamiento es sencillo y se puede entender como un for que recorre las propiedades de un objeto. En el ejemplo quiere decir que se crea la variable propiedad `let propiedad` que va a recorrer cada propiedad del objeto `persona` con el `in` y luego se imprime la propiedad y el valor de la propiedad.

Esto significa que al recorrer el objeto `persona` con un bucle `for...in`, se imprimirá cada propiedad del objeto en la consola. En este caso, se imprimirán las propiedades `nombre: Juan`, `edad: 30` y `casado: false`.

cosas a tener en cuenta:

- Se utiliza un bucle `for...in` para recorrer el objeto. El ```for...in``` es solo para objetos, no para arreglos.
- La variable `propiedad` se utiliza para acceder a cada propiedad del objeto.
- La expresión `persona[propiedad]` se utiliza para acceder al valor de cada propiedad del objeto.
- Se puede utilizar el bucle `for...in` para realizar operaciones con cada propiedad del objeto, como imprimirlas, modificarlas, eliminarlas, y más.

### Retos

- Realizar un programa que reciba un objeto con las propiedades `nombre`, `edad`, `casado` y devuelva un mensaje con la información de la persona.
- Realizar un programa que reciba un objeto con las propiedades `nombre`, `edad`, `casado` y devuelva un mensaje con la información de la persona, pero si la persona está casada, devolver un mensaje diferente.
- Realizar un programa que reciba un objeto con las propiedades `nombre`, `edad`, `casado` y devuelva un mensaje con la información de la persona, pero si la persona es mayor de edad, devolver un mensaje diferente.
- Realizar un programa que reciba un objeto con las propiedades `nombre`, `edad`, `casado` y devuelva un mensaje con la información de la persona, pero si la persona es mayor de edad y está casada, devolver un mensaje diferente.
- Realizar un programa que reciba un objeto con las propiedades `nombre`, `edad`, `casado` y devuelva un mensaje con la información de la persona, pero si la persona es mayor de edad y está casada, devolver un mensaje diferente, y si la persona es menor de edad y está soltera, devolver un mensaje diferente.