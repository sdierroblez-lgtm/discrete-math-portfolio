# 🔹 Fase 1: Fundamentos de la Teoría de Grafos

Bienvenido a la primera fase de la Unidad 3. En esta sección documento mi introducción práctica a las estructuras de datos no lineales. El objetivo principal de esta fase es comprender cómo modelar relaciones mediante nodos (vértices) y aristas, y cómo un sistema informático recorre estas estructuras de manera sistemática.

---

## 🪐 1. Modelado y Representación Básica

Para iniciar, transformamos conceptos abstractos en representaciones visuales y matemáticas. 

### Grafo del Sistema Solar
Este fue el modelado inicial donde los nodos representan los cuerpos celestes y las aristas dictan las conexiones o relaciones espaciales entre ellos. Para que el computador pueda procesar esta red, acompañamos el gráfico con su respectiva **Matriz de Adyacencia**.

> **📷 Evidencia del Modelado:**
> 
> ![Diagrama del Grafo del Sistema Solar](<img width="595" height="582" alt="Grafo del Sistema Solar" src="https://github.com/user-attachments/assets/89990be8-cc1d-40f5-820f-efdad7824439" />
)

---

## 🔍 2. Algoritmos de Recorrido y Búsqueda

Saber cómo transitar de un nodo a otro de manera óptima es vital en la computación. A continuación, presento las trazas manuales (el paso a paso) de los dos algoritmos de búsqueda elementales, comprobando la lógica de las estructuras de datos que los operan.

### 🌊 Búsqueda en Anchura (BFS - Breadth-First Search)
Este algoritmo explora el grafo de manera concéntrica, revisando todos los vecinos de un nodo antes de pasar al siguiente nivel.
*   **Estructura de memoria utilizada:** Cola (FIFO - *First In, First Out*).

> **📷 Traza Manual BFS:**
> 
> ![Tabla paso a paso BFS](nombre_de_tu_imagen_bfs.jpg)

### 🕳️ Búsqueda en Profundidad (DFS - Depth-First Search)
Este método avanza agresivamente hacia el fondo de una trayectoria. Solo cuando llega a un "callejón sin salida" retrocede (*backtracking*) para explorar otras ramas.
*   **Estructura de memoria utilizada:** Pila (LIFO - *Last In, First Out*).

> **📷 Traza Manual DFS:**
> 
> ![Tabla paso a paso DFS](nombre_de_tu_imagen_dfs.jpg)

---

### 💡 Conclusión de la Fase 1
El desarrollo de estas trazas manuales fue fundamental para comprender que la elección entre una Pila o una Cola cambia por completo el comportamiento de un sistema de navegación o búsqueda de datos.

---
[⬅️ Volver al Menú Principal](../../README.md)
