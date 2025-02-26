## Algoritmos básicos y lógica de programación

Vamos a entrar en un tema muy importante en la programación, los algoritmos. Un algoritmo es un conjunto de instrucciones o reglas que se utilizan para resolver un problema o realizar una tarea. Los algoritmos son la base de la programación, ya que permiten dividir un problema en partes más pequeñas y fáciles de entender, y luego combinar esas partes para obtener una solución.

Entonces la idea es mejorar la lógica de programación, y para eso vamos a realizar una serie de ejercicios que nos ayudarán a mejorar la lógica de programación y a entender cómo se resuelven problemas con algoritmos.

### Importancia de pseudocódigo

El pseudocódigo es una forma de escribir algoritmos en un lenguaje sencillo y comprensible, que se utiliza para planificar y diseñar programas antes de escribir el código en un lenguaje de programación. El pseudocódigo es muy útil para organizar las ideas, definir los pasos a seguir, y resolver problemas de forma clara y estructurada.

El pseudocódigo se utiliza para describir los pasos que se deben seguir para resolver un problema, sin preocuparse por la sintaxis de un lenguaje de programación específico. El pseudocódigo se puede escribir en cualquier idioma, pero se recomienda utilizar un lenguaje sencillo y claro para que sea fácil de entender.

Veamos un ejemplo:

Problema: Realizar un programa que busque un número en un arreglo y devuelva la posición del número si se encuentra, o -1 si no se encuentra.

Recordar que un computador entiende es objeto por objeto, posición por posición, entonces a veces nuestra mente puede pensar en un problema de una forma más abstracta, pero el computador necesita instrucciones claras y precisas. Por ejemplo, si tenemos un arreglo de 5 elementos, y queremos buscar un número, nuestra mente puede pensar como pues ahí en la mitad del arreglo, pero el computador necesita instrucciones claras y precisas, como recorrer el arreglo, comparar el número con cada elemento, si encuentra el número, devolver la posición, si no encuentra el número, devolver -1.

```plaintext

Inicio

Definir un arreglo de números
Definir un número a buscar

Para cada elemento del arreglo
    Si el elemento es igual al número a buscar
        Devolver la posición del elemento
    Fin Si
Fin Para

Devolver -1

Fin

```

Este es un ejemplo de pseudocódigo para el problema de buscar un número en un arreglo. Como puedes ver, el pseudocódigo describe los pasos que se deben seguir para resolver el problema, sin preocuparse por la sintaxis de un lenguaje de programación específico. El pseudocódigo es muy útil para planificar y diseñar programas antes de escribir el código en un lenguaje de programación. Recuerda lo que dije una vez, entender el lenguaje natural puede ayudarnos a observar que hay palabras que de una vez su interpretación nos ayuda para saber que estructura de control debemos utilizar, por ejemplo, si vemos la palabra "si" sabemos que es una estructura de control condicional, si vemos la palabra "para" sabemos que es una estructura de control de bucle, y así sucesivamente.

Entonces que sucede, la programación no es definitiva, es decir, no hay una sola forma de resolver un problema, entonces si tu tienes una forma de resolver un problema, y otra persona tiene otra forma de resolver el problema, no significa que una sea mejor que la otra, sino que son diferentes formas de resolver el problema. (Por el momento vamos a decir que ninguna es mejor que la otra, pero en la programación hay algo que se llama eficiencia, y es importante tener en cuenta la eficiencia de un algoritmo, pero eso lo veremos más adelante; o bueno, en la vida real, a veces podemos encontrar una forma de resolver un problema que sea más eficiente que otra, pero eso no significa que la otra forma sea mala, sino que es menos eficiente).

### Retos

Vamos a realizar pseudocódigo e implementar.

- Realizar un programa que busque un número en un arreglo y devuelva la posición del número si se encuentra, o -1 si no se encuentra.
- Ordenar un arreglo de números de menor a mayor.
- Ordenar un arreglo de números de mayor a menor.
- Realizar un programa que dado un arreglo aleatorio de números, me diga de alguna forma cuantos numeros hay de cada uno. Es decir, ejemplo me diga cuantos 1, cuantos 2, cuantos 3, y así sucesivamente.
- Escribe un programa que imprima los números del 1 al 100, pero en los múltiplos de 3 imprime "Fizz", en los múltiplos de 5 "Buzz", y en los múltiplos de ambos "FizzBuzz".
- Crea una función que encuentre el número más grande en un arreglo.
- Dado un string, escribe una función que cuente cuántas vocales contiene.
- Dada una palabra, imprimir la palabra al revés (Derecha a izquierda).