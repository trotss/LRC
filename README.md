# Prueba de Concepto (PoC) de Código LRC [6,4,2]
Este repositorio contiene una Prueba de Concepto (PoC) de un código de paridad localmente recuperable (LRC) con parámetros [6,4,2]. El objetivo principal de esta PoC es evaluar el rendimiento en términos de tiempos de codificación, decodificación y recuperación para diferentes escenarios de fallos de shards (fragmentos de datos).

---
## Descripción del Código LRC [6,4,2]
Un código LRC [n, k, r] se define de la siguiente manera:
n: Número total de shards (fragmentos) codificados.
k: Número de shards de datos originales.
r: Número de grupos de paridad local.
En este caso, para un código [6,4,2]:
Tenemos 6 shards totales.
4 shards son de datos originales.
Se utilizan 2 grupos de paridad local, lo que significa que la recuperación de un shard perdido se puede hacer usando un conjunto más pequeño de shards de paridad.

---
## Evaluación de Tiempos
La PoC evalúa los siguientes tiempos de operación:
Tiempo de Codificación: El tiempo que tarda el algoritmo en generar los 6 shards (4 de datos y 2 de paridad) a partir de los 4 shards de datos originales.
Tiempo de Decodificación: El tiempo que se requiere para reconstruir los 4 shards de datos originales a partir de los shards codificados disponibles, asumiendo que no hay pérdidas.
Tiempo de Recuperación de 1 Shard: El tiempo para recuperar un único shard de datos perdido utilizando la paridad local o global.
Tiempo de Recuperación de 2 Shards: El tiempo para recuperar dos shards de datos perdidos, demostrando la capacidad del código para manejar múltiples fallos.

No hay requeriments.txt, gestiónatelo.
