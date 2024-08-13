# Factorial
El factorial de un número entero no negativo 𝑛 es el producto de todos los enteros positivos menores o iguales a 𝑛. Se denota como 𝑛! (n factorial). El factorial se define de la siguiente manera:
- **Caso base**:
>  El factorial de 0 es 1, es decir, 0!=1.
- **Caso Recursivo**:
> Para cualquier número entero positivo 𝑛, el factorial se calcula como 𝑛!=𝑛×(𝑛−1)!
### Ejemplos de factoriales:
- 0! = 1 (por definición)
- 1! = 1
- 2! = 2 \times 1 = 2
- 3! = 3 \times 2 \times 1 = 6
- 4! = 4 \times 3 \times 2 \times 1 = 24
- 5! = 5 \times 4 \times 3 \times 2 \times 1 = 120
## Aplicaciones del Factorial:
El concepto de factorial tiene varias aplicaciones en matemáticas y computación:
- Combinatoria:
  > Se utiliza para contar las permutaciones y combinaciones de conjuntos. Por ejemplo, el número de maneras diferentes de organizar 𝑛 objetos es 𝑛!
- Series Matemáticas:
  > Aparece en el desarrollo de series de Taylor y en otros tipos de series matemáticas.
- Probabilidad y Estadística:
  > Es útil para calcular probabilidades en problemas que involucran permutaciones y combinaciones.
- Algoritmos y Computación:
  > La computación del factorial se usa en algoritmos relacionados con la teoría de grafos, optimización y análisis de algoritmos.
## Calculo de Factorial en distintos lenguajes:
- *Kotlin* :
~~~
  fun factorial(n: Int): Int {
    return if (n <= 1) 1 else n * factorial(n - 1)
}
fun main() {
    println(factorial(5))  // Salida: 120
}
 ~~~
- *Python* :
~~~
def factorial(n):
    if n <= 1:
        return 1
    else:
        return n * factorial(n - 1)

print(factorial(5))  # Salida: 120
~~~
- *Java* :
~~~
function factorial(n) {
    if (n <= 1) return 1;
    return n * factorial(n - 1);
}

console.log(factorial(5));  // Salida: 120
~~~
## Consideraciones:
- Crecimiento Exponencial:
> El factorial de un número crece muy rápido. Por ejemplo, 20! es un número con 19 dígitos.
- Límites Computacionales:
> Debido al rápido crecimiento del factorial, las operaciones pueden superar los límites de almacenamiento para números muy grandes en algunos lenguajes de programación, por lo que se deben usar tipos de datos especiales o técnicas de manejo de grandes enteros en esos casos.

**El factorial es una función matemática fundamental con muchas aplicaciones prácticas y teóricas, y es un concepto básico en el estudio de la combinatoria y la teoría de algoritmos.**
