# Graph_generation_spm
# Author: Sergio Pérez Montes
# Análisis y diseño de algoritmos
Biblioteca de Modelos de Grafos
Esta biblioteca proporciona una implementación para varios modelos de generación de grafos en Python. Incluye modelos como Malla (Grid), Erdős-Rényi, 
Gilbert, Geográfico, Barabási-Albert y Dorogovtsev-Mendes, ofreciendo una gama de herramientas para crear y analizar diferentes tipos de estructuras 
de grafos.

Características
Grafo de Malla: Genera grafos de malla con dimensiones especificadas.
Modelo Erdős-Rényi: Crea grafos añadiendo aristas entre vértices de manera aleatoria.
Modelo Gilbert: Genera grafos aleatorios donde cada par de nodos se conecta con cierta probabilidad.
Modelo Geográfico: Produce grafos colocando vértices en un cuadrado unitario y conectando pares que se encuentran dentro de una distancia especificada.
Modelo Barabási-Albert: Crea redes libres de escala utilizando un mecanismo de adjunción preferencial.
Modelo Dorogovtsev-Mendes: Genera grafos comenzando con un triángulo y añadiendo nuevos vértices conectados a dos vértices existentes elegidos al azar.

Instalación
Para utilizar esta biblioteca, simplemente incluye el archivo Python en tu proyecto o impórtalo directamente si estás trabajando en un entorno que soporte scripts de Python.

Uso
Creando un Grafo de Malla

malla_grafo = grafoMalla(m, n, dirigido=False)
Generando un Grafo Erdős-Rényi

ER_grafo = grafoErdosRenyi(n, m, dirigido=False)
Grafo Modelo Gilbert

Gilbert_grafo = grafoGilbert(n, p, dirigido=False)
Grafo Modelo Geográfico

geografico_grafo = grafoGeografico(n, r, dirigido=False)
Grafo Modelo Barabási-Albert

BA_grafo = grafoBarabasiAlbert(n, d, dirigido=False)
Grafo Modelo Dorogovtsev-Mendes

DM_grafo = grafoDorogovtsevMendes(n, dirigido=False)

Exportando a GraphViz
Cada modelo incluye un método para exportar el grafo generado a un archivo .gv de GraphViz, permitiendo una visualización fácil:

malla_grafo.exportar_graphviz("malla_grafo")
Requisitos
Python 3.x

Módulos random y math (incluidos con la instalación estándar de Python)

