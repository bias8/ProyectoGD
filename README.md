[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=bias8/ProyectoGD)
# Proyecto: Modelo matemático de poblaciones celulares

### Información de los estudiantes

* Alberto Villalobos Valdez [22212277]; L22212277@tectijuana.edu.mx
* Bricia Idalia Arellano Salones [22211746]; L22211746@tectijuana.edu.mx
* Biología de Sistemas / Gemelos Digitales
* Ingeniería Biomédica

### Docente

* Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx
* Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

### Descripción de la asignatura

La asignatura de Gemelos Digitales forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Formula el gemelo digital a través de datos experimentales para el desarrollo estrategias de control mediante teorías de sistemas dinámicos no lineales y la experimentación in silico. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional.

En el contexto de sistemas dinámicos que describen sistemas biológicos o fisiológicos, el modelizado in silico es una extensión lógica de la experimentación in vitro controlada, es el resultado natural del gran aumento de la potencia computacional disponible a un costo que disminuye continuamente, combinando las ventajas de la experimentación in vivo e in vitro, sin someterse a las consideraciones éticas y la falta de control asociadas con los experimentos in vivo. A diferencia de los experimentos in vitro, que existen de forma aislada, los modelos in silico permiten incluir un conjunto prácticamente ilimitado de variables y parámetros, lo que hace que los resultados sean más aplicables en problemas del mundo real. La experimentación in silico ha dado lugar al paradigma denominado como "gemelos digitales" (en inglés digital twins); en esencia, los gemelos digitales son una réplica o representación digital de un proceso o sistema del mundo real, donde por replica se refiere a un modelo computacional desarrollado con base en datos experimentales y características especiales que le permiten conectar lo físico con lo virtual con el propósito de mejorar el rendimiento de un sistema, detectar y prevenir fallas, y realizar predicciones sobre su respuesta ante diferentes estímulos o escenarios de operación; una definición más formal establece que: un gemelo digital es un conjunto de modelos adaptativos que emulan el comportamiento de un sistema físico en un sistema virtual obteniendo datos en tiempo real para actualizarse a lo largo de su ciclo de vida; replica al sistema físico para predecir fallas y oportunidades de cambio, prescribir acciones en tiempo real para optimizar y/o mitigar eventos inesperados observando y evaluando el perfil operativo del sistema. En el campo particular de la Biología de Sistemas, un gemelo digital se presenta como un algoritmo o conjunto de algoritmos computacionales desarrollados con base en modelos mecanicistas de un organismo vivo, esto con el objetivo de emular su fisiología para ilustrar su dinámica en el corto y en el largo plazo, así como predecir su respuesta a diferentes estímulos endógenos y exógenos.

### Objetivo y descripción del sistema
<img width="1427" height="727" alt="image" src="https://github.com/user-attachments/assets/24946b70-8ada-4727-b39a-8465b2a98872" />

Un tipo particular de sistema dinámico es aquel que exhibe diferentes conjuntos compactos invariantes para diferentes valores en sus parámetros y/o condiciones iniciales. A continuación, se presenta un modelo matemático que describe la dinámica entre tres poblaciones celulares, el cual está compuesto por las siguientes tres EDOs no lineales de primer orden:

$$\dot{x} = a_1 x^2 y z - a_2 x - a_3 x^2 y$$

$$\dot{y} = b_1 y - b_2 y^2 - b_3 y^3$$

$$\dot{z} = c_1 x z - c_2 z - c_3 y^2 z^2 + \rho_i$$

donde todos los parámetros son estrictamente positivos y se asume una dinámica controlada por un parámetro de inmunoterapia o intervención de control dado por $i \geq 0$. La Ecuación (1) representa la evolución de la población patológica ($x$), la Ecuación (2) describe la población de células sanas ($y$) con una dinámica de crecimiento controlada por sus propios parámetros poblacionales, y la Ecuación (3) modela la respuesta del sistema biológico o de células efectoras ($z$). El análisis de este sistema permite evaluar la positividad de las poblaciones y buscar la eliminación de la condición patológica.

**Palabras clave:** EDO; Modelo matemático; PID; Gemelos digitales; Poblaciones celulares.

### Actividades a realizar

* Demostrar analíticamente la positividad del sistema en el dominio $\mathbb{R}^3_{+,0}$ garantizando la viabilidad biológica del modelo.
* Calcular los puntos de equilibrio del sistema, particularmente aquellos que representan el estado libre de células patológicas.
* Analizar la estabilidad asintótica local del sistema evaluando la matriz Jacobiana en sus puntos de equilibrio.
* Determinar los valores propios de la matriz para establecer las condiciones matemáticas que garantizan la estabilidad de las poblaciones.

### Lista de archivos incluidos en el repositorio

* Cuaderno computacional de MATLAB [.mlx].
* Análisis matemático y de estabilidad [.pdf].
* Imágenes de las simulaciones y retrato fase [.pdf].
* Diagrama de bloques/biológico del sistema [.png].

### Referencias

[1] P. A. Valle, Syllabus para Gemelos Digitales, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2026. Permalink: [https://biomath.xyz/course/](https://biomath.xyz/course/)

[2] De Leenheer, P., & Aeyels, D. (2001). Stabilization of positive linear systems. Systems & Control Letters, 44(4), 259-271.

[3] Bryan, Kurt. Differential equations: A toolbox for modeling the world. Simiode, 2022. Permalink: [https://www.simiode.org/resources/8307](https://www.simiode.org/resources/8307)

[4] E. Toscano, E. Cimmino, A. Boccia, L. Sepe, and G. Paolella, “Cell populations simulated *in silico* within SimulCell accurately reproduce the behaviour of experimental cell cultures,” *npj Systems Biology and Applications*, vol. 11, no. 1, p. 48, 2025. doi: 10.1038/s41540-025-00518-w.
