|               |                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Fecha         | 04 de septiembre de 2025                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Audio         | [OneDrive](https://alumnosuady-my.sharepoint.com/personal/a19203594_alumnos_uady_mx/_layouts/15/stream.aspx?id=%2Fpersonal%2Fa19203594%5Falumnos%5Fuady%5Fmx%2FDocuments%2FSemestres%2FSemestre%20VII%2FExperimentaci%C3%B3n%20en%20Ingenier%C3%ADa%20de%20Software%2FClases%2FGrabaciones%2Fexper%5Fvera%5F2025%2E09%2E04%2Em4a&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E8147e96d%2D93d0%2D45d7%2D812e%2D1f306d4640c3) :lock: |
| Transcripción | [../raw/exper_vera_2025.09.04.m4a.txt](../raw/exper_vera_2025.09.04.m4a.txt)                                                                                                                                                                                                                                                                                                                                                                                  |

# Principios del Diseño Experimental y Calidad de la Medición

**Resumen**

La clase se enfocó en dos áreas principales: la calidad de la medición y los principios fundamentales del diseño experimental. Se comenzó repasando las escalas de medición (nominal, ordinal, de intervalo y de razón) y su relación con la elección de pruebas estadísticas paramétricas y no paramétricas. Posteriormente, se introdujeron tres conceptos clave para evaluar la calidad de una métrica: **precisión**, **fiabilidad** (confiabilidad) y **validez**. La segunda parte de la sesión se dedicó a explicar los cuatro principios básicos para un diseño experimental robusto: **repetición**, **aleatorización**, **formación de bloques** y **factorización**, detallando el propósito y la aplicación de cada uno con ejemplos prácticos en el contexto de la ingeniería de software.

**Palabras Clave:** 
Diseño Experimental, Escalas de Medición, Precisión, Fiabilidad, Validez, Repetición, Aleatorización, Bloqueo, Factorización, ANOVA, Pruebas Paramétricas.

## Reporte Detallado

La sesión inició con un repaso de la teoría de la medición, enfatizando la importancia de las escalas y su impacto en el análisis estadístico posterior.

### Calidad de la Medición

Se discutieron tres características esenciales que toda métrica debe poseer para ser útil en un experimento:

1.  **Precisión:** Se refiere al nivel de detalle de una medida, usualmente relacionado con el número de dígitos o decimales utilizados. Una mayor precisión permite capturar variaciones más finas, pero se debe tener en cuenta que al realizar operaciones aritméticas con medidas de precisión limitada, el resultado puede ser aún menos preciso.

2.  **Fiabilidad (o Confiabilidad):** Mide la consistencia de los resultados de una medición al ser repetida en condiciones similares. Es especialmente crucial para medidas subjetivas (ej. encuestas de opinión, evaluación de usabilidad). Un instrumento es fiable si diferentes evaluadores llegan a conclusiones similares o si el mismo evaluador obtiene resultados consistentes en distintos momentos. Se mencionó el **alfa de Cronbach** como un índice común para medir la fiabilidad de los instrumentos tipo cuestionario.

3.  **Validez:** Es el grado en que una métrica realmente mide lo que se supone que debe medir. Se discutieron tres tipos de validez:
    *   **Validez de Contenido:** La métrica debe reflejar adecuadamente el dominio del atributo que se pretende medir. (Ej. La complejidad de un programa no debe basarse en el idioma en que están escritos los identificadores).
    *   **Validez de Criterio:** La métrica debe reflejar una relación coherente con un criterio externo. (Ej. La definición de "inteligencia" debe estar clara para que la métrica sea válida).
    *   **Validez de Constructo:** Es la más importante y se refiere a si la métrica mide el concepto teórico abstracto correcto. (Ej. No confundir la medición de *eficacia* con la de *eficiencia*).

### Principios del Diseño Experimental

El núcleo de la clase fue la explicación de los cuatro pilares que sustentan un buen diseño experimental, diseñados para gestionar la variabilidad y asegurar que las conclusiones sean robustas.

1.  **Repetición (Replication):**
    *   **Definición:** Consiste en realizar el experimento más de una vez, es decir, tener múltiples unidades experimentales para cada tratamiento. No se trata de que una persona repita la tarea, sino de que varias personas la realicen.
    *   **Propósito:** Permite obtener una estimación más precisa del error experimental y aumenta la potencia del experimento para detectar diferencias significativas entre los tratamientos. A mayor número de repeticiones (mediciones), más confianza se tiene en los resultados.

2.  **Aleatorización (Randomization):**
    *   **Definición:** Es la asignación de los sujetos experimentales a los diferentes tratamientos al azar.
    *   **Propósito:** Busca promediar el efecto de factores no controlados (ruido o variables extrañas) de manera equitativa entre todos los tratamientos. Transforma la variabilidad sistemática no planificada en error aleatorio, previniendo sesgos.
    *   **Ejemplo:** Si se tienen 12 estudiantes y 2 técnicas (A y B), se asignan aleatoriamente 6 estudiantes a la técnica A y 6 a la técnica B para que factores como la inteligencia o la motivación se distribuyan de forma equilibrada.

3.  **Formación de Bloques (Blocking):**
    *   **Definición:** Es una técnica para controlar una fuente de variabilidad conocida que no es el factor de interés principal. Consiste en agrupar las unidades experimentales en "bloques" homogéneos y luego asignar los tratamientos de forma aleatoria dentro de cada bloque.
    *   **Propósito:** Aumenta la precisión del experimento al eliminar la variabilidad causada por el factor de bloqueo.
    *   **Ejemplo:** Si se sabe que el nivel de *expertise* (experto vs. inexperto) influye en el resultado al probar dos técnicas, se crean dos bloques: uno con todos los expertos y otro con los inexpertos. Dentro de cada bloque, se asignan aleatoriamente las técnicas A y B. Esto asegura que ambas técnicas sean probadas por igual número de expertos e inexpertos.

4.  **Factorización en el Diseño (Factorial Design):**
    *   **Definición:** Es una estrategia para estudiar el efecto de dos o más factores simultáneamente en un solo experimento.
    *   **Propósito:** Es más eficiente que realizar experimentos separados para cada factor y, fundamentalmente, permite estudiar las **interacciones** entre los factores (es decir, si el efecto de un factor depende del nivel de otro).
    *   **Ejemplo:** Se quiere estudiar el efecto de 3 técnicas de revisión (Factor 1: A, B, C) y 2 niveles de complejidad del código (Factor 2: Sencillo, Complejo). Un diseño factorial probaría las 3x2=6 combinaciones (tratamientos) posibles.

### Preguntas y Aclaraciones Relevantes

- **¿Cuándo se usaría una prueba estadística para una sola muestra?**
  Se aclaró que este diseño se utiliza cuando se compara el resultado de un grupo experimental contra un **estándar o valor de referencia preexistente**, en lugar de compararlo contra otro grupo.

- **¿Cuál es la diferencia entre Aleatorización y Bloqueo?**
  La **aleatorización** se usa para controlar los efectos de variables extrañas **desconocidas** o que no se pueden medir, distribuyendo su impacto al azar. El **bloqueo** se utiliza para controlar el efecto de una variable **conocida y medible** que influye en la respuesta pero que no es el foco principal del estudio.

## Indicaciones Académicas

*   **ADA sobre Medición (para el viernes):** Se recuerda que está pendiente la entrega de la actividad sobre medición. Se aclaró que los conceptos de precisión, fiabilidad y validez, necesarios para completar la tarea, se encuentran en el segundo material de lectura cargado en la plataforma (identificado como 6B o 7B), específicamente en la sección 3.2.