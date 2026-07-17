#  Fase 4: Proyecto Integrador - Modelado y Optimización de Redes

##  INFORME TÉCNICO: Teoría de grafos para optimizar la red de cobertura a instituciones educativas públicas de la Provincia Sur del Sumapaz (Colombia)

---

### 1. Descripción del Problema

*   **Contexto y Relevancia:** La Universidad de Cundinamarca, sede Fusagasugá, desarrolla proyectos de Ciencia, Tecnología e Innovación (CTI) e interacción social universitaria (ISU), como talleres de robótica educativa y pensamiento computacional. Estos programas buscan atender las necesidades de instituciones educativas públicas en la Provincia del Sumapaz; sin embargo, se ha identificado que la cobertura actual se limita a los municipios cercanos, excluyendo a poblaciones de zonas rurales y apartadas.
*   **El Desafío Técnico:** La región presenta una geografía montañosa compleja y una infraestructura vial precaria, caracterizada por carreteras rurales no pavimentadas y en mal estado. Estas condiciones generan un desafío logístico significativo, traduciéndose en altos costos y un uso considerable de tiempo para el traslado de recurso humano y tecnológico.
*   **Objetivos:** El estudio se propone determinar las rutas de viaje más rápidas desde la Universidad de Cundinamarca (sede Fusagasugá) hacia las instituciones educativas públicas más apartadas de la Provincia Sur del Sumapaz para optimizar la planificación de actividades y la asignación de recursos.

---

###  2. Modelado Matemático y Teórico

*   **Lógica / Álgebra Booleana:** No especificado en el artículo original.
*   **Teoría de Grafos:** El problema se modela mediante un grafo simple y ponderado definido formalmente como:
    $$G = (V, E)$$
*   **Vértices ($V$):** Representan 13 ubicaciones estratégicas, incluyendo la sede universitaria (nodo origen), municipios, centros poblados y veredas de la región.
*   **Aristas ($E$):** Representan las conexiones viales reales entre los nodos seleccionados (16 aristas en total).
*   **Pesos ($w$):** El peso de cada arista $w(u,v)$ corresponde al tiempo promedio de viaje expresado estrictamente en minutos.

---

###  3. Implementación en Software

*   **Arquitectura:** La solución está estructurada mediante la recolección de datos de tiempos de viaje reales y su posterior procesamiento mediante un modelo de grafos para la ejecución de algoritmos de optimización.
*   **Algoritmos y Lógica:** Se implementa el **Algoritmo de Dijkstra**, el cual opera en tres fases principales:
    1.  Marcación del nodo origen con tiempo cero.
    2.  Exploración de vértices adyacentes y cálculo o actualización de tiempos acumulados.
    3.  Selección del vértice no visitado con el peso mínimo para la siguiente iteración.
*   **Tecnologías Utilizadas:**
    *   **Google Maps:** Utilizado para la obtención de los tiempos de viaje reales entre los diferentes nodos de la red.
    *   **Python:** Lenguaje empleado para desarrollar la aplicación lógica encargada de estructurar el grafo y ejecutar el algoritmo de Dijkstra.

---

### 📊 4. Resultados Obtenidos

Se analizaron cuatro recorridos estratégicos desde el nodo origen (FU - Fusagasugá) hacia los destinos más alejados de la provincia, evaluando alternativas de conexión vial para asegurar la ruta mínima absoluta.

| Recorrido | Origen | Ruta Óptima | Destino Final | Tiempo Total (min) |
| :---: | :---: | :--- | :---: | :---: |
| **1** | FU | $\text{FU} \rightarrow \text{SI} \rightarrow \text{TI} \rightarrow \text{CU}$ | Cumaca | 59 min |
| **2** | FU | $\text{FU} \rightarrow \text{EB} \rightarrow \text{BA}$ | Bateas | 68 min |
| **3** | FU | $\text{FU} \rightarrow \text{EB} \rightarrow \text{PA} \rightarrow \text{VE} \rightarrow \text{CA}$ | Cabrera | 146 min |
| **4** | FU | $\text{FU} \rightarrow \text{AR} \rightarrow \text{SB} \rightarrow \text{SH} \rightarrow \text{AN}$ | Vereda Andes | 150 min |



---

###  5. Análisis de Optimización

La aplicación sistemática del algoritmo de Dijkstra permitió descartar rutas intuitivas que resultaban menos eficientes debido al estado de las vías. 
*   **Caso Bateas:** Para llegar a Bateas se comparó la ruta tradicional vía Cumaca (que tomaba entre 100 y 110 minutos) con la ruta optimizada vía El Boquerón ($\text{EB}$), obteniendo una reducción drástica del tiempo de viaje a solo **68 minutos**.
*   **Caso Cabrera:** Para el tercer recorrido, la ruta óptima arrojó **146 minutos**, superando con éxito a otras alternativas evaluadas por el sistema que registraban tiempos de 177 y 232 minutos respectivamente.

---

###  6. Conclusiones

*   **Conclusiones del Autor:** Se demuestra empíricamente que la teoría de grafos y el algoritmo de Dijkstra constituyen métodos eficaces y confiables para optimizar rutas logísticas en contextos rurales complejos. El modelo proporciona una base cuantitativa sólida para la planificación de proyectos universitarios en zonas de difícil acceso.
*   **Limitaciones y Trabajo Futuro:** Los tiempos calculados se centran exclusivamente en el traslado vial y no consideran la duración de las visitas técnicas dentro de cada institución. El artículo original no especifica otras líneas de desarrollo futuro.

---
[⬅️ Volver al Menú Principal](../../README.md)
