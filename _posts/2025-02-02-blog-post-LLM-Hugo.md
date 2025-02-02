---
title: 'De Victor Hugo hacia los Large Language Models'
date: 2025-02-02
permalink: /posts/2025/02/blog-post-1/
tags:
  - ChatGPT
  - Large Language Models
  - Lógica
---

# De Victor Hugo hacia los Large Language Models

![Ilustración de Victor Hugo](https://revista.marketing/images/Efemerides/Febrero_2021/26-de-febrero-1802-Nace-Victor-Hugo-ilustracion-ia-inspirada.jpg)

*Imagen tomada de [Revista Marketing](https://revista.marketing/efemerides/21-cultura/367-26-de-febrero-nace-victor-hugo). Derechos reservados a sus respectivos autores.*

En 1862, el novelista y poeta francés Victor Hugo publica su maravillosa
obra “Los Miserables”, un relato que anima constantes debates sobre el
bien, el mal, la justicia y la ley. En uno de sus primeros episodios se
retrata la casa del obispo de Digne, cuyos únicos tesoros consistían en
seis cubiertos de plata, un cucharón y dos grandes candelabros de plata
maciza. Como una muestra de la humildad de este personaje, Hugo relata
que repetidamente comentaba que “difícilmente renunciaría a comer con
cubiertos que no fuesen de plata”.

Quizá el detallista lector pueda descifrar prontamente su significado.
Otros como yo, requerimos su revisión y algunos segundos de razón con un
análisis a partir de estas tres frases:

1.  Si renuncio a comer con cubiertos que son de plata 🡪 Deseo comer con
    cubiertos de estaño.

2.  Si renuncio a comer con cubiertos que no son de plata 🡪 Deseo comer
    con cubiertos que son de plata.

3.  Si difícilmente renuncio a comer con cubiertos que no son de plata 🡪
    No deseo comer con cubiertos que son de plata.

Entretanto, hay quienes sin mayor meditación balbucean que “el obispo no
tenía hambre” o que “quería otro plato”, en muestras inherentes de
cierto letargo en la razón.

Lo cierto es que este silogismo requiere de un proceso de deconstrucción
para su comprensión. “Difícilmente renunciar” es una doble negación que
significa la afirmación de aceptar. Por lo tanto, el obispo de Digne
está dispuesto a comer con cubiertos que no son de plata, en
concordancia con el marco de austeridad en que lo ubica Hugo.

Ahora bien, como un simple ejercicio de curiosidad, he suministrado esta
cuestión a dos aplicativos de inteligencia artificial: ChatGPT y
DeepSeek, y los resultados no son nada satisfactorios.

![Imagen3](https://github.com/user-attachments/assets/9d0828b0-af43-4467-84c4-a3a40a142a09)
<p>Respuesta generada por ChatGPT. 2025-02-02. </p>  

![Imagen2](https://github.com/user-attachments/assets/6aa9d1d7-5466-45d3-8666-76c0c089b51e)
<p>Respuesta generada por DeepSeek. 2025-02-02. </p>  

¿Por qué resulta que estos dos poderosos *Large Language Models* (LLM),
capaces de construir complejos códigos algorítmicos, redactar ensayos
sobre filosofía o construir ingeniosas campañas de publicidad, fallen
ante una pregunta que requiere algo de raciocinio?

Encontré la respuesta en la investigación del profesor [Binghui
Peng](https://www.cs.columbia.edu/~binghuip/) de la Universidad de
Columbia, quien con su equipo de trabajo se concentró en la pregunta de
por qué los LLM presentan estas respuestas confusas, también conocidas
como alucinaciones. Para comprender su trabajo debemos establecer que
este tipo de problemas son llamados “tareas de composición complejas” y
se caracterizan por que la solución a un problema consiste en la
solución de múltiples subproblemas que a su vez también son resultado de
la solución de otros subproblemas, en una compleja relación de capas de
subproblemas. Algo muy parecido a las estrategias de solución utilizadas
en [programación dinámica en el campo de la optimización
matemática](https://en.wikipedia.org/wiki/Dynamic_programming).

Peng y su equipo lograron demostrar que los transformadores multicapa
(que vienen a ser estructuras de redes neuronales en las que se basan
los LLM) [no pueden resolver ciertas tareas de composición complejas, y
demostraron](https://arxiv.org/abs/2402.08164) que, si el número total
de parámetros en un transformador es menor que el tamaño del dominio,
probablemente ese transformador no pueda resolver tareas de composición
complejas. En otras palabras, existe una limitación matemática para los
transformadores que ejecutan tareas en los LLM.

Este hallazgo es complementado con el estudio de la profesora [Nohura
Dziri](https://nouhadziri.github.io/) del Allen Institute for Artificial
Intelligence en su trabajo sobre los [límites de los transformadores en
las tareas de composición](https://arxiv.org/pdf/2305.18654) en donde se
sugiere que los transformadores LLM resuelven estas tareas mediante un
proceso de “comparación linealizada de subgrafos”, sin desarrollar
necesariamente un razonamiento sistemático. En síntesis, los LLM “pueden
no ser capaces de razonar mas allá de aquello que han visto durante las
tareas de entrenamiento con datos”.

Los científicos buscan enfrentar estas limitantes de los LLM a través de
mecanismos que no impliquen el rediseño de toda la arquitectura
desarrollada. Técnicas como las [“cadenas de pensamiento”
(chain-of-thought)](https://www.quantamagazine.org/how-chain-of-thought-reasoning-helps-neural-networks-compute-20240321/)
prometen ayudar a las redes neuronales a resolver problemas de este
tipo.

Para finalizar, el profesor Anil Ananthaswamy, autor del [artículo sobre
el que baso este
post](https://www.quantamagazine.org/chatbot-software-begins-to-face-fundamental-limitations-20250131/)
pone las cosas en su lugar. Mientras que la gran mayoría de usuarios
continuarán utilizando los LLM para resolver tareas sencillas que
facilitan su productividad, otros en la comunidad científica buscan
comprender “qué es lo que sucede tras bambalinas” y cómo se dan esos
procesos de solución de tareas con interrogantes acerca del “cómo lo
hacen” antes de “qué es lo que hacen”.

Mientras tanto, me atrevo a afirmar que “con gran pesar aceptaría la
posibilidad de no preferir abiertamente que Los miserables continúe
planteando interrogantes que ahora van más desde los no prohibidos
espacios de la justicia, la ética y la moral, hacia el abierto uso y sin
desdén en los campos de la ciencia de la información”.

