
# ¿Es Rust una opción viable para simular computación cuántica en sistemas clásicos?
BSc. Daniel Jaimes, Ph.D Gabriel Pedraza

logo de la UIS a la derecha

## Introducción y Contexto

### La computación cuántica: un desafío y una oportunidad
La computación cuántica combina física avanzada y matemáticas complejas, lo que exige lenguajes eficientes para simular sus principios en hardware clásico.
Aunque hoy en día lenguajes como C, Python o Julia lideran en este campo, Rust ofrece un enfoque único gracias a su rendimiento, seguridad y control de memoria.

### Rust y la computación cuántica: un futuro por construir
El ecosistema actual de Rust para la computación cuántica es pequeño, pero sus características fundamentales podrían hacer de este lenguaje una alternativa prometedora en simulación cuántica y gestión de hardware especializado.


## Algunas características de Rust

### Rust frente a los desafíos cuánticos
Simular sistemas cuánticos implica trabajar con vectores de alta dimensión, álgebra lineal y cálculos extremadamente precisos. Rust ofrece características clave para este tipo de tareas:

- **Rendimiento de bajo nivel:** Compilación directa a máquina, ideal para cálculos matemáticos intensivos.
- **Seguridad garantizada:** Prevención de errores como data races y problemas de memoria, esenciales para sistemas complejos.
- **Concurrencia avanzada:** Ejecución paralela eficiente y segura, facilitando simulaciones más rápidas.
- **Extensibilidad:** Su capacidad de trabajar con C/C++ lo hace ideal para futuros desarrollos híbridos.

### Un paralelismo interesante
El borrow checker de Rust refleja principios cuánticos como el teorema de no clonación, asegurando que no se puedan duplicar estados arbitrariamente, lo que lo hace un lenguaje atractivo desde una perspectiva conceptual.

## Metodología y Ejemplos
### Metodología
En esta exploración, se realizaron implementaciones básicas de algoritmos cuánticos clásicos para experimentar la viabilidad de Rust como lenguaje en simulaciones de computación cuántica. Si bien no se buscó optimizar al máximo ni desarrollar herramientas altamente complejas, estas implementaciones ofrecen un punto de partida para futuras pruebas y desarrollos más avanzados.

El enfoque consistió en:

- **Simular circuitos cuánticos básicos:** Construcción de estados cuánticos y puertas básicas como Hadamard, Pauli-X y CNOT.
- **Implementar algoritmos fundamentales:** Como el algoritmo de Grover y el algoritmo de Deutsch-Josza.
- **Explorar características avanzadas:** Manejo de oracles (funciones clásicas que condicionan las operaciones cuánticas), mediciones y entrelazamiento.
- 
### Algoritmos implementados

#### Algoritmo de Grover
Grover es un algoritmo de búsqueda cuántica que encuentra elementos en bases de datos no ordenadas con una complejidad cuadrática menor que los algoritmos clásicos.

Característca en Rust:
- Manejo eficiente de operaciones iterativas, esenciales en la construcción del oráculo y la inversión sobre el promedio.
- Seguridad del borrow checker para prevenir inconsistencias al actualizar estados cuánticos.

#### Algoritmo de Deutsch-Josza
Este algoritmo decide si una función es constante o equilibrada con una sola evaluación, destacando las ventajas de la superposición cuántica.

Caraterística en Rust:
- Modularidad y claridad al modelar funciones binarias como oracles.
- La concurrencia permite simular evaluaciones de funciones paralelas eficientemente.

#### Circuitos cuánticos básicos
Se trabajó en la construcción y simulación de puertas cuánticas comunes como:
- Puerta Hadamard (H): Genera superposición uniforme.
- Puerta CNOT: Introduce entrelazamiento.
- Puerta T y S: Importantes para realizar correcciones de fase.

Característica en Rust:
- Definición de puertas como funciones puras, facilitando su reutilización y asegurando su comportamiento determinista.

#### Oracles y mediciones
Los oracles son fundamentales en algoritmos como Grover, ya que representan funciones clásicas utilizadas en circuitos cuánticos.

Ventaja en Rust:
- Capacidad de definir oráculos como cierres (closures) o funciones genéricas que respetan restricciones de seguridad y optimización.
- Control explícito de la memoria durante mediciones, asegurando que los resultados no afecten estados futuros no deseados.

---
Imagen central del Logo Rust y Ferris en efecto glitch, posiblemente con circuitos cuanticos difuminados en el fondo
---

## Más características que hacen a Rust relevante

### Borrow Checker y No-cloning Theorem
La regla de préstamo en Rust tiene similitudes conceptuales con el teorema de no clonación en computación cuántica, que establece que no es posible clonar un estado cuántico desconocido. Esto facilita modelar sistemas cuánticos de forma que se garantice la consistencia del estado.

### Concurrencia segura
Simular sistemas cuánticos requiere realizar operaciones independientes en paralelo, especialmente al evaluar múltiples caminos en un circuito.
- Rust permite manejar hilos de forma segura, reduciendo errores como condiciones de carrera (race conditions).

### Rendimiento y memoria controlada
Rust permite trabajar cerca del hardware, optimizando recursos de memoria y asegurando que los cálculos cuánticos simulados no se vean limitados por overhead innecesario, como podría ocurrir en lenguajes interpretados.

### Flexibilidad para estructuras de datos
Los sistemas cuánticos suelen representarse mediante matrices densas o dispersas, vectores complejos y otras estructuras matemáticas avanzadas.
- Rust facilita la implementación de estas estructuras utilizando bibliotecas como ndarray o nalgebra, combinadas con macros y funciones puras para garantizar eficiencia.

### Macros para abstracciones elegantes
Aunque las macros no fueron el foco principal de esta exploración, Rust permite abstraer constructos cuánticos comunes en bloques de código reutilizables, que se asemejan a la notación utilizada en libros de texto. Esto simplifica la construcción de circuitos más complejos.

## Reflexión y Trabajo a Futuro

**¿Es Rust una opción para el futuro cuántico?**  
Aunque el ecosistema de Rust para computación cuántica es menos maduro en comparación con otros lenguajes, su adopción podría ser estratégica a largo plazo. Crear herramientas y bibliotecas basadas en Rust no solo ofrecería una alternativa segura y eficiente, sino que también abriría nuevas posibilidades para gestionar hardware cuántico con mayor control.

**Trabajo a futuro**

1.  Puede ser la base para un nuevo ecosistema cuántico, donde el rendimiento y la seguridad sean críticos.
2.  Desarrollar bibliotecas que exploten las fortalezas de Rust en campos matemáticos.
5.  Su adopción abriría oportunidades para herramientas más robustas en simulación y hardware híbrido.
6.  Fomentar su desarrollo ahora podría convertirlo en una pieza clave en sistemas de computación avanzada en el futuro.


---
Imagenes
Logo de Rust programming
https://asamaci.org.ar/wp-content/uploads/2024/10/Logo-Maci-1-300x300.png
Ferris Rust (Cangrejo)
Circuitos cuanticos
Naranja similar a Ferris #F07430
122cm (height) and 92cm (width)

holi
