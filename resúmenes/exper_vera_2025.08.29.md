|               |                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Fecha         | 29 de agosto de 2025                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Audio         | [OneDrive](https://alumnosuady-my.sharepoint.com/personal/a19203594_alumnos_uady_mx/_layouts/15/stream.aspx?id=%2Fpersonal%2Fa19203594%5Falumnos%5Fuady%5Fmx%2FDocuments%2FSemestres%2FSemestre%20VII%2FExperimentaci%C3%B3n%20en%20Ingenier%C3%ADa%20de%20Software%2FClases%2FGrabaciones%2Fexper%5Fvera%5F2025%2E08%2E29%2Em4a&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Eba4cdb36%2D7830%2D480f%2Dabc9%2D9d5f06da2c82) :lock: |
| Transcripción | [../raw/exper_vera_2025.08.29.m4a.txt](../raw/exper_vera_2025.08.29.m4a.txt)                                                                                                                                                                                                                                                                                                                                                                                  |

# Teoría de la Medición y Escalas de Medición en Ingeniería de Software

**Resumen**

La clase se dedicó a establecer los fundamentos de la teoría de la medición aplicada a la ingeniería de software. Utilizando una analogía histórica sobre el problema de medir la longitud en la navegación, se destacó la crucial importancia y dificultad de la medición, especialmente en un campo donde los productos no son tangibles. Se definieron conceptos clave como **medición** (el proceso de asignación), **medida** (el valor asignado, también llamado **métrica**), **entidad** (los objetos a medir: productos, procesos y recursos) y **atributo** (la característica de interés). El foco principal de la sesión fue la explicación detallada de las cuatro escalas de medición —**Nominal, Ordinal, de Intervalo y de Razón**—, describiendo para cada una sus propiedades, las operaciones matemáticas admisibles y su relevancia para el análisis estadístico, subrayando que la elección de la escala impacta directamente la profundidad de la información que se puede derivar.

**Palabras Clave:** 
Medición, Escalas de Medición, Escala Nominal, Escala Ordinal, Escala de Intervalo, Escala de Razón, Métrica, Atributo, Entidad de Software.

## Reporte Detallado

La sesión comenzó con una reflexión sobre la dificultad histórica de la medición, ejemplificada por el desafío de calcular la longitud geográfica en el mar, para introducir la problemática similar en la ingeniería de software, donde la intangibilidad de los productos añade una capa de complejidad.

### Conceptos Fundamentales de la Medición

Se establecieron las definiciones formales que sustentan el proceso de medición:

*   **Entidades:** Son los "objetos" del mundo real que se desean medir en el contexto del software. Se clasifican principalmente en tres categorías:
    1.  **Productos (o Artefactos):** Entregables del proceso, como el código fuente, documentos de requisitos o diagramas de diseño.
    2.  **Procesos:** El conjunto de actividades y tareas realizadas por los individuos, como el proceso de pruebas o de diseño.
    3.  **Recursos:** Elementos necesarios para llevar a cabo el proyecto, como las personas (desarrolladores), el tiempo y el costo.

*   **Atributo:** Es una característica o propiedad específica de una entidad que se quiere medir. Por ejemplo, el `tamaño` es un atributo de la entidad `código`.

*   **Medición:** Es el proceso formal mediante el cual se asigna un número o un símbolo (una medida) a un atributo de una entidad, siguiendo una regla bien definida.

*   **Medida (o Métrica):** Es el valor resultante del proceso de medición. Por ejemplo, `400` es la medida del atributo `tamaño` de un código, donde la métrica utilizada son las `líneas de código`.

### Escalas de Medición

El núcleo de la clase fue la descripción de los cuatro niveles o escalas de medición, que determinan el tipo de información que contiene una medida y las operaciones que se pueden realizar con ella.

1.  **Escala Nominal:**
    *   **Descripción:** Es la escala más básica. Asigna nombres o etiquetas para clasificar entidades en categorías distintas. No hay un orden implícito entre las categorías.
    *   **Operaciones:** Igualdad (`==`) y desigualdad (`!=`).
    *   **Ejemplos:** Lenguaje de programación (Java, Python, C++), tipo de defecto.
    *   **Indicador de Tendencia Central:** Moda.

2.  **Escala Ordinal:**
    *   **Descripción:** Los valores de esta escala tienen un orden o ranking. Permite saber si un atributo es "mayor que" o "menor que" otro, pero no la magnitud de la diferencia entre ellos.
    *   **Operaciones:** Las de la escala nominal más orden (`<`, `>`).
    *   **Ejemplos:** Nivel de expertise (Junior, Semi-Senior, Senior), grado de madurez CMMI (Nivel 1, 2, 3), escalas Likert (Totalmente en desacuerdo, ..., Totalmente de acuerdo).
    *   **Indicador de Tendencia Central:** Mediana.

3.  **Escala de Intervalo:**
    *   **Descripción:** Es una escala ordenada donde la distancia (intervalo) entre valores consecutivos es constante y significativa. Sin embargo, no posee un cero absoluto o verdadero (el cero es un punto arbitrario en la escala).
    *   **Operaciones:** Las de la escala ordinal más suma (`+`) y resta (`-`).
    *   **Ejemplos:** Temperatura en grados Celsius, fechas del calendario. No es común en la ingeniería de software.
    *   **Indicador de Tendencia Central:** Media.

4.  **Escala de Razón:**
    *   **Descripción:** Es la escala de medición más potente. Posee todas las propiedades de la escala de intervalo, pero además cuenta con un **cero absoluto**, que indica la ausencia total del atributo. Permite establecer proporciones (ej. "el doble de", "la mitad de").
    *   **Operaciones:** Todas las operaciones aritméticas (`+`, `-`, `*`, `/`).
    *   **Ejemplos:** Número de líneas de código, costo del proyecto en pesos, tiempo de ejecución en segundos, número de defectos encontrados.
    *   **Indicador de Tendencia Central:** Media.

Se enfatizó que para las variables dependientes en un experimento, es altamente deseable utilizar escalas de razón, ya que permiten aplicar un rango más amplio y potente de técnicas estadísticas.

### Otras Clasificaciones de Medidas

Finalmente, se mencionaron brevemente otras formas de clasificar las medidas:
*   **Directas vs. Indirectas:** Las directas se obtienen sin cálculos intermedios (ej. contar líneas de código). Las indirectas se derivan de otras medidas (ej. velocidad = distancia/tiempo).
*   **Objetivas vs. Subjetivas:** Las objetivas no dependen del observador (ej. tiempo de compilación). Las subjetivas implican un juicio o apreciación (ej. calificar la calidad de un diseño).
*   **Atributos Internos vs. Externos:** Los internos son propios de la entidad (ej. complejidad ciclomática de un código). Los externos se refieren a cómo la entidad se relaciona con su entorno (ej. la usabilidad del software para un usuario).

### Preguntas y aclaraciones relevantes

*   **¿Son significativas todas las operaciones matemáticas con números?**
    Se aclaró que no. Una operación solo es significativa si el resultado tiene una correspondencia en el mundo real. Se usó el ejemplo de multiplicar la probabilidad de un accidente por el impacto del mismo, cuyo resultado numérico no tiene un significado real, en contraste con dividir distancia entre tiempo para obtener velocidad, que sí lo tiene.

*   **¿Qué implica que una escala sea más "poderosa" que otra?**
    Una escala es más poderosa si permite realizar más operaciones y, por lo tanto, derivar más información. No se puede afirmar que un "nivel 4" de expertise es el doble de un "nivel 2" (escala ordinal), pero sí se puede afirmar que un código de "400 líneas" es el doble de grande que uno de "200 líneas" (escala de razón).

## Indicaciones Académicas

*   **Tarea para la próxima sesión (jueves):**
    *   Pensar en un **producto**, un **recurso** y un **proceso** del ámbito de la ingeniería de software.
    *   Para cada uno, proponer un atributo a medir y describir:
        1.  En qué **escala de medición** estaría (Nominal, Ordinal, de Intervalo o de Razón).
        2.  Si la medida es **directa o indirecta**.
        3.  Si la medida es **objetiva o subjetiva**.
        4.  Si el atributo es **interno o externo**.
    *   Se proporcionará una guía en la plataforma para estructurar la entrega.