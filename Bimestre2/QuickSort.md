# QuickSort

## ¿Qué es QuickSort?

QuickSort es un algoritmo de ordenamiento basado en el paradigma **Divide y vencerás**. Su eficiencia proviene de dividir inteligentemente el problema en partes más pequeñas y ordenar cada una de manera recursiva.

## ¿Cómo funciona?

1. **Elegir un pivote**: Se selecciona un elemento de la lista, llamado *pivote*.
2. **Particionar**: Se reordenan los elementos de tal manera que todos los menores al pivote estén a su izquierda y los mayores a su derecha.
3. **Ordenar recursivamente**: Se aplica el mismo procedimiento a las sublistas izquierda y derecha.

## Representación general del algoritmo

```pseudo
función quickSort(lista, inicio, fin):
    si inicio < fin:
        índicePivote = particionar(lista, inicio, fin)
        quickSort(lista, inicio, índicePivote - 1)
        quickSort(lista, índicePivote + 1, fin)

función particionar(lista, inicio, fin):
    pivote = lista[fin]
    i = inicio - 1
    para j desde inicio hasta fin - 1:
        si lista[j] < pivote:
            i += 1
            intercambiar(lista[i], lista[j])
    intercambiar(lista[i + 1], lista[fin])
    retornar i + 1
