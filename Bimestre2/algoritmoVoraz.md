# Algoritmo Voraz – Problema del Cambio de Monedas

Este documento explica el uso de un algoritmo voraz para resolver el problema del cambio de monedas. La actividad consistió en aplicar una estrategia de elección óptima local para obtener la combinación mínima de monedas posibles que sumen una cantidad determinada.

## ¿Qué es un algoritmo voraz?

Un algoritmo voraz (greedy) es un enfoque que toma decisiones paso a paso eligiendo siempre la mejor opción disponible en ese momento, sin preocuparse por cómo esa elección afectará decisiones futuras.

Este tipo de algoritmo es útil para resolver problemas de optimización donde se busca la solución más eficiente, rápida o barata, aunque no siempre garantiza el resultado óptimo global.

## Problema planteado: cambio de monedas

**Objetivo:** Dado un conjunto de monedas y un monto total, seleccionar la menor cantidad de monedas posible para dar el cambio.

**Conjunto de monedas utilizado:**  
[50, 20, 10, 5, 1]

### Caso 1: Monto = 60

**Estrategia aplicada:**
- Tomar 1 moneda de 50 → faltan 10
- Tomar 1 moneda de 10 → faltan 0

**Total de monedas usadas: 2**

### Caso 2: Monto = 99

**Estrategia aplicada:**
- 1 × 50 → queda 49  
- 2 × 20 → queda 9  
- 1 × 5 → queda 4  
- 4 × 1 → queda 0

**Total de monedas usadas: 8**

## Análisis del algoritmo

**Ventajas:**
- Rápido y fácil de implementar.
- Requiere poca memoria y lógica simple.

**Desventajas:**
- No siempre garantiza la mejor solución global.
- Puede fallar si las denominaciones de monedas no están bien diseñadas para un enfoque voraz.

En este caso específico, el algoritmo sí dio una solución eficiente. Sin embargo, en otros conjuntos de monedas, como [1, 3, 4], puede dar resultados subóptimos.

## Conclusiones

- El algoritmo voraz fue útil y eficaz para resolver los casos dados.
- Las pruebas de escritorio permitieron verificar su comportamiento paso a paso.
- Es importante probar estos algoritmos con distintos escenarios, ya que su efectividad depende del diseño del conjunto de decisiones posibles.

## Recomendaciones

- Si se requiere una solución siempre óptima, se recomienda usar enfoques como programación dinámica.
- En sistemas reales, como cajeros automáticos o cajas registradoras, se debe validar que el sistema monetario sea compatible con estrategias voraces.

Este taller permitió reforzar la comprensión de los algoritmos voraces, su eficiencia y sus limitaciones frente a casos más complejos.
