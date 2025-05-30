## Algoritmos

Semana 1: Algoritmia Elemental
Objetivo: Conocer las características, componentes y notación de un algoritmo.Contenido:  

Preliminares: Introducción a los algoritmos, notación, contradicción, inducción matemática y resolución de problemas.  
Ejemplo Básico:Un algoritmo para calcular el factorial de un número n:  Entrada: n (entero positivo)
Salida: n! (factorial de n)
1. Si n = 0, devolver 1
2. Sino, devolver n * factorial(n-1)

Este algoritmo usa recursión y su notación se puede expresar como una recurrencia.  
Actividades:  
Presentación en clase del plan docente y del tema.  
Análisis práctico de la importancia de los algoritmos mediante ejemplos.  
Tarea autónoma: Configurar un repositorio en GitHub y leer textos (Cormen et al., 2022: "The Role of Algorithms in Computing"; Brassard & Bratley, 2006: "Preliminares").Propósito: Establecer una comprensión fundamental de los algoritmos como concepto central en computación.



Semana 2: Eficiencia de Algoritmos y Caso Medio
Objetivo: Profundizar en las características y notación de algoritmos, enfocándose en la eficiencia.Contenido:  

Eficiencia de Algoritmos: Técnicas para medir el rendimiento.  
Análisis del Caso Medio: Comportamiento de algoritmos en entradas típicas.  
Ejemplo Básico:Comparación de dos algoritmos para buscar un elemento en una lista:  
Búsqueda lineal: Recorre cada elemento hasta encontrarlo (O(n)).  def busqueda_lineal(lista, objetivo):
    for i in range(len(lista)):
        if lista[i] == objetivo:
            return i
    return -1


Comparar tiempos de ejecución para listas de diferentes tamaños.


Actividades:  
Discusión en clase y análisis de complejidad de algoritmos simples.  
Taller comparando tiempos de ejecución de algoritmos.  
Lectura autónoma: Cormen et al. (2022): "Insertion Sort"; Brassard & Bratley (2006): "Algoritmia Elemental".Propósito: Introducir la evaluación del rendimiento de algoritmos mediante análisis teórico y práctico.



Semana 4: Notación Asintótica (Orden de Crecimiento)
Objetivo: Comprender el costo en tiempo y espacio de algoritmos en diversos escenarios.Contenido:  

Notación Asintótica: Introducción a la notación "Big O" para describir la complejidad.  
Ejemplo Básico:Análisis de un algoritmo de suma de una lista:  def suma_lista(lista):
    total = 0
    for num in lista:
        total += num
    return total

Complejidad: O(n), donde n es el tamaño de la lista, ya que se recorre una vez.  
Actividades:  
Presentación en clase y ejemplos de notación asintótica.  
Evaluación parcial sobre la Unidad 1.  
Ejercicios prácticos definiendo modelos matemáticos con Big O.  
Tarea autónoma: Revisar y analizar casos de algoritmos.Propósito: Dotar a los estudiantes de herramientas para cuantificar el rendimiento de algoritmos.



Semana 5: Caracterización de Tiempos de Ejecución
Objetivo: Analizar costos en tiempo y espacio usando notaciones asintóticas avanzadas.Contenido:  

Notaciones Omega y Theta: Cotas inferiores y ajustadas de complejidad.  
Notación Asintótica Condicional: Aplicación en escenarios específicos.  
Ejemplo Básico:Para el algoritmo de suma de lista (Semana 4):  
Big O: O(n) (cota superior).  
Omega: Ω(n) (cota inferior, debe recorrer al menos todos los elementos).  
Theta: Θ(n) (cota ajustada, recorre exactamente n elementos).


Actividades:  
Presentación en clase y desarrollo de ejercicios.  
Taller práctico aplicando Omega y Theta.  
Lectura autónoma y resolución de problemas.Propósito: Profundizar en el análisis asintótico para una evaluación precisa.



Semana 6: Análisis de Algoritmos (Estructuras de Control)
Objetivo: Analizar costo y complejidad de algoritmos usando modelos matemáticos.Contenido:  

Estructuras de Control: Impacto de bucles y condicionales en la eficiencia.  
Ejemplo Básico:Análisis de un bucle anidado para encontrar el máximo de una matriz:  def max_matriz(matriz):
    maximo = matriz[0][0]
    for i in range(len(matriz)):
        for j in range(len(matriz[0])):
            if matriz[i][j] > maximo:
                maximo = matriz[i][j]
    return maximo

Complejidad: O(n*m), donde n y m son las dimensiones de la matriz.  
Actividades:  
Presentación en clase y desarrollo de ejercicios.  
Ejercicios prácticos aplicando notaciones a estructuras de control.  
Preparación autónoma para evaluaciones.Propósito: Modelar y analizar la eficiencia según el flujo de control.



Semana 7: Análisis de Algoritmos (Caso Medio, Análisis Amortizado y Recurrencias)
Objetivo: Analizar costo y complejidad usando modelos matemáticos avanzados.Contenido:  

Análisis del Caso Medio: Evaluación del rendimiento típico.  
Análisis Amortizado: Rendimiento a largo plazo en múltiples operaciones.  
Recurrencias: Resolver relaciones para algoritmos recursivos.  
Ejemplo Básico:Recurrencia para el factorial recursivo:  def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n-1)

Recurrencia: T(n) = T(n-1) + O(1), resuelve a T(n) = O(n).  
Actividades:  
Presentación en clase y desarrollo de ejercicios.  
Taller aplicando análisis del caso medio y recurrencias.  
Lectura autónoma: Brassard & Bratley (2006): "Notación Asintótica".  
Tarea: Desarrollar y actualizar casos en el repositorio de GitHub.Propósito: Proporcionar herramientas avanzadas para analizar algoritmos recursivos y amortizados.




Referencias:  

Cormen, T. H., Leiserson, C. E., Rivest, R. L., & Stein, C. (2022). Introduction to Algorithms (4th ed.). The MIT Press.  
Brassard, G., & Bratley, P. (2006). Fundamentals of Algorithmics.

Este resumen alinea los resultados de aprendizaje del curso, preparando a los estudiantes para analizar problemas computacionales y proponer soluciones usando métodos matemáticos.
