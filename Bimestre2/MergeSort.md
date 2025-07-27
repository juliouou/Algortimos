# Merge Sort
## ¿Qué es Merge Sort?

Merge Sort es un algoritmo de ordenamiento que aplica la estrategia de **Divide y vencerás**. Consiste en dividir recursivamente una lista en mitades hasta que cada sublista tenga un solo elemento, y luego ir **combinando (merging)** estas sublistas de manera ordenada hasta reconstruir la lista completa en orden.

## ¿Cómo funciona?

1. **División**: Se divide la lista en dos mitades.
2. **Conquista**: Se ordenan recursivamente ambas mitades usando el mismo algoritmo.
3. **Combinación**: Se fusionan ambas mitades ordenadas en una nueva lista ordenada.

## Representación general del algoritmo

```pseudo
función mergeSort(lista):
    si longitud(lista) ≤ 1:
        retornar lista
    mitad = longitud(lista) / 2
    izquierda = mergeSort(lista[0:mitad])
    derecha = mergeSort(lista[mitad:])
    retornar merge(izquierda, derecha)

función merge(izquierda, derecha):
    resultado = []
    mientras izquierda y derecha no estén vacías:
        si izquierda[0] < derecha[0]:
            agregar izquierda[0] a resultado
            eliminar izquierda[0]
        sino:
            agregar derecha[0] a resultado
            eliminar derecha[0]
    agregar elementos restantes de izquierda y derecha a resultado
    retornar resultado
