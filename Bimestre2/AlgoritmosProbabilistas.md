# Algoritmos Probabilistas
## ¿Qué es un algoritmo probabilista?

Un algoritmo probabilista es aquel que, en una o más de sus etapas, **hace uso de valores aleatorios (números al azar)** como parte de su lógica de decisión. Debido a esto, el algoritmo puede producir resultados distintos incluso si se ejecuta varias veces con la misma entrada.

## ¿Para qué se usan los algoritmos probabilistas?

Estos algoritmos son especialmente útiles cuando:

- Se trabaja con **grandes volúmenes de datos**.
- Es costoso o imposible encontrar una solución exacta.
- Se requiere obtener **una solución rápida y aceptablemente buena**.
- No existe una forma determinista eficiente para resolver el problema.

Son comunes en áreas como:

- Criptografía
- Compresión de datos
- Inteligencia artificial
- Teoría de números
- Simulación y análisis estadístico
- Procesamiento de señales

## Tipos de algoritmos probabilistas

### 1. Algoritmos de Monte Carlo

- Devuelven una respuesta que puede ser incorrecta con cierta probabilidad.
- **Controlan el tiempo de ejecución**, pero sacrifican precisión.
- Ejemplo clásico: Prueba de primalidad de Miller-Rabin.

### 2. Algoritmos de Las Vegas

- Siempre devuelven una **respuesta correcta**, pero el tiempo de ejecución es **probabilístico**.
- En ocasiones puede tomar más tiempo debido a que depende de resultados aleatorios.

## Ventajas

- Son rápidos en promedio.
- Son más simples que muchos algoritmos deterministas equivalentes.
- En muchos casos son la única alternativa práctica para problemas muy complejos.

## Desventajas

- Su comportamiento no es completamente predecible.
- Requieren una fuente confiable de números aleatorios.
- No garantizan la mejor solución en todos los casos (en los algoritmos de Monte Carlo).

## Ejemplo conceptual: búsqueda aleatoria

Supongamos que queremos encontrar un número `x` dentro de una lista grande de `n` elementos.

Un algoritmo probabilista puede simplemente elegir índices al azar hasta encontrar `x`, en lugar de recorrer toda la lista de manera secuencial. Aunque esto puede parecer ineficiente, en ciertas condiciones puede ofrecer buen rendimiento promedio, especialmente si `x` aparece muchas veces o si la lista cambia dinámicamente.

## Conclusión

Los algoritmos probabilistas representan una forma poderosa y flexible de resolver problemas que, de otra manera, serían muy difíciles de abordar con algoritmos deterministas. Aunque no siempre garantizan una solución exacta o un tiempo de ejecución fijo, su simplicidad y eficiencia promedio los hace muy útiles en aplicaciones prácticas.

Este tema complementa los paradigmas estudiados durante el bimestre, mostrando cómo la aleatoriedad también puede utilizarse como una herramienta efectiva para diseñar soluciones algorítmicas.
