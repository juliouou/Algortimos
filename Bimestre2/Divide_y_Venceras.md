# Divide y Vencerás – Búsqueda Binaria

## ¿Qué es el paradigma Divide y Vencerás?

El paradigma Divide y Vencerás consiste en resolver un problema dividiéndolo en subproblemas más pequeños, resolviendo cada uno por separado, y combinando sus soluciones.

Este enfoque es útil cuando el problema original puede descomponerse naturalmente y cada parte puede resolverse de forma similar a la original. Se aplica ampliamente en algoritmos como Merge Sort, QuickSort y Búsqueda Binaria.

## Aplicación: Búsqueda Binaria

La Búsqueda Binaria es un algoritmo que permite encontrar un elemento en una lista ordenada de manera eficiente. Utiliza el paradigma Divide y Vencerás al reducir a la mitad el rango de búsqueda en cada paso.

**Ventaja principal:** Su complejidad es logarítmica, es decir, O(log n), lo que la hace mucho más eficiente que una búsqueda secuencial cuando los datos están ordenados.

## Prueba de escritorio

**Tupla de entrada:**  
T = [8, 10, 14, 24, 28, 35, 49, 56, 98]

**Elemento a buscar:**  
x = 14

**Pasos del algoritmo:**

1. Inicio = 0, Fin = 8  
   Mitad = (0 + 8) // 2 = 4 → T[4] = 28  
   Como 14 < 28, buscar a la izquierda.

2. Fin = 3  
   Mitad = (0 + 3) // 2 = 1 → T[1] = 10  
   Como 14 > 10, buscar a la derecha.

3. Inicio = 2, Fin = 3  
   Mitad = (2 + 3) // 2 = 2 → T[2] = 14  
   Elemento encontrado.

**Resultado:**  
x = 14 se encuentra en la posición 2 del arreglo.

## Implementación básica

El algoritmo se puede implementar de forma iterativa o recursiva. Ambos métodos aplican el mismo principio de dividir el rango de búsqueda hasta encontrar el elemento o agotar las posibilidades.

```java
public static int busquedaBinaria(int[] arreglo, int x) {
    int inicio = 0;
    int fin = arreglo.length - 1;

    while (inicio <= fin) {
        int mitad = (inicio + fin) / 2;

        if (arreglo[mitad] == x)
            return mitad;
        else if (x < arreglo[mitad])
            fin = mitad - 1;
        else
            inicio = mitad + 1;
    }
    return -1; // No encontrado
}
