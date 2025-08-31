|               |                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Fecha         | 21 de agosto de 2025                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Audio         | [OneDrive](https://alumnosuady-my.sharepoint.com/personal/a19203594_alumnos_uady_mx/_layouts/15/stream.aspx?id=%2Fpersonal%2Fa19203594%5Falumnos%5Fuady%5Fmx%2FDocuments%2FSemestres%2FSemestre%20VII%2FExperimentaci%C3%B3n%20en%20Ingenier%C3%ADa%20de%20Software%2FClases%2FGrabaciones%2Fexper%5Fvera%5F2025%2E08%2E21%2Em4a&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E866da061%2D1122%2D406f%2Db4c3%2D1ea27c985719) :lock: |
| Transcripción | [../raw/exper_vera_2025.08.21.mp3.txt](../raw/exper_vera_2025.08.21.mp3.txt)                                                                                                                                                                                                                                                                                                                                                                                 |

# Métodos de Investigación Empírica en Ingeniería de Software

**Resumen**

La clase se centró en los métodos de investigación empírica aplicados a la ingeniería de software, partiendo de la definición de la disciplina como un enfoque sistemático, disciplinado y cuantificable. Se utilizó un ejemplo detallado sobre la revisión de código en pruebas unitarias para explicar conceptos clave de la experimentación, como la identificación y control de variables (dependientes, independientes y extrañas), la formulación de hipótesis y la importancia de la significancia estadística. Posteriormente, se presentó una clasificación de los métodos de investigación según su propósito (exploratorios, descriptivos, explicativos, de mejora), el tipo de datos (cuantitativos vs. cualitativos), el diseño (fijos vs. flexibles) y la fuente de evidencia (primarios vs. secundarios). Finalmente, se describieron los métodos más comunes en el área: experimentos, encuestas, estudios de caso e investigación-acción, destacando sus características y contextos de aplicación.

**Palabras Clave:** 
Investigación Empírica, Experimentación, Variables (Dependiente, Independiente), Control de Variables, Prueba de Hipótesis, Métodos Cuantitativos, Métodos Cualitativos, Estudio de Caso, Encuesta, Ingeniería de Software.

## Reporte Detallado

La sesión comenzó repasando la definición fundamental de la Ingeniería de Software, destacando su enfoque **sistemático, disciplinado y cuantificable** como base para la mejora continua y la toma de decisiones. Se estableció que el contexto para la investigación empírica son los proyectos de desarrollo de software, donde los conceptos teóricos se materializan.

### El Proceso Experimental: Un Ejemplo Práctico

Para ilustrar los conceptos de la experimentación, se analizó un escenario hipotético: comparar la efectividad de una técnica de revisión de código tradicional (en papel) contra una innovadora (asistida por herramienta) durante las pruebas unitarias. Este ejemplo sirvió para identificar y discutir los siguientes elementos:

1.  **Variable Independiente:** Es la variable que el investigador manipula intencionadamente. En este caso, es la **técnica de revisión de código** utilizada (Tradicional vs. Innovadora).
2.  **Variable Dependiente:** Es la variable que se mide para observar el efecto de la manipulación. Aquí, podría ser la **efectividad** (número de faltas detectadas) o la **eficiencia** (número de faltas detectadas por unidad de tiempo).
3.  **Variables a Controlar (Parámetros):** Son otros factores que podrían influir en el resultado y deben ser homogeneizados para que no sesguen el experimento. Se identificaron:
    *   **El Personal (Tester):** Su nivel de experiencia (*expertise*) es crucial. Se debe controlar asegurando que los participantes tengan un nivel similar o que el mismo sujeto realice ambas tareas (diseño de muestras relacionadas vs. independientes).
    *   **El Código:** Características como el número de líneas, el lenguaje de programación y la complejidad del algoritmo deben ser las mismas para todos los participantes.
    *   **El Proceso:** Las instrucciones y el entorno deben ser idénticos para todos, salvo por la técnica que se está probando.

### Clasificación de Métodos de Investigación

Se presentaron diversas formas de clasificar los métodos de investigación utilizados en la disciplina:

*   **Según el Propósito:**
    1.  **Exploratoria:** Cuando se conoce poco del fenómeno. Busca generar ideas e hipótesis.
    2.  **Descriptiva:** Describe las características y relaciones entre variables conocidas.
    3.  **Explicativa:** Busca confirmar relaciones de causa y efecto entre variables. Aquí se ubican los experimentos.
    4.  **De Mejora:** Intenta mejorar un aspecto del fenómeno mientras se realiza la investigación (ej. Investigación-Acción).

*   **Según el Tipo de Datos:**
    *   **Cuantitativos:** Utilizan datos numéricos y análisis estadístico. Son objetivos y buscan generalizar resultados (ej. Experimentos, Encuestas con preguntas cerradas).
    *   **Cualitativos:** Se basan en datos no numéricos como opiniones y comportamientos. Son subjetivos y buscan una comprensión profunda (ej. Estudios de Caso, Entrevistas abiertas).

*   **Según el Diseño y la Evidencia:**
    *   **Diseño Fijo vs. Flexible:** Los métodos fijos (cuantitativos) se planean a detalle y no se modifican, mientras que los flexibles (cualitativos) se adaptan durante su ejecución.
    *   **Primarios vs. Secundarios:** Los primarios generan nueva evidencia enfrentándose al fenómeno (ej. un experimento), mientras que los secundarios analizan evidencia ya existente (ej. una revisión de literatura).

### Métodos Principales en Ingeniería de Software

*   **Experimentos:** Estudian relaciones causa-efecto manipulando variables en un entorno controlado.
*   **Encuestas:** Recopilan información estandarizada de una muestra para generalizarla a una población.
*   **Estudios de Caso:** Investigan a fondo un fenómeno en su contexto real, sin controlar variables. Es ideal para evaluar una herramienta o proceso en un proyecto específico.
*   **Investigación-Acción:** Similar al estudio de caso, pero el investigador participa activamente para cambiar y mejorar el proceso estudiado.

Finalmente, se mencionó la tendencia actual de usar **métodos mixtos**, combinando enfoques cuantitativos y cualitativos para obtener una comprensión más completa y robusta del fenómeno de estudio.

### Preguntas y aclaraciones relevantes

-  **¿La asignación de propósitos a una investigación (exploratoria, descriptiva, etc.) es análoga a los objetivos de una tesis?**
    Sí, el propósito de la investigación define en gran medida el tipo y alcance del trabajo de tesis. Una tesis de doctorado, por ejemplo, busca generar conocimiento nuevo (explicativo/de mejora), mientras que una de licenciatura podría ser una revisión documental (descriptiva) o la aplicación de una técnica conocida en un nuevo contexto.

-  **¿Cómo se traduce una hipótesis de investigación a una hipótesis estadística?**
    La hipótesis de investigación (ej. "la técnica nueva es mejor que la tradicional") se traduce en un par de hipótesis estadísticas: la **hipótesis nula (H₀)**, que plantea que no hay diferencia significativa entre las técnicas, y la **hipótesis alternativa (H₁)**, que plantea que sí la hay. El objetivo del análisis estadístico es intentar rechazar la hipótesis nula.

-  **¿Cuál es la diferencia entre efectividad y eficiencia como variables dependientes?**
    La **efectividad** se refiere a qué tan bien se logra el objetivo (ej. el número total de faltas encontradas). La **eficiencia** relaciona la efectividad con los recursos utilizados, particularmente el tiempo (ej. número de faltas encontradas por hora).

## Indicaciones Académicas

*   **Registro en Plataforma:** Se solicita a los alumnos que aún no lo han hecho, registrarse en el curso en la plataforma Moodle.
*   **ADA 1.1 - Reporte sobre Fases del Proceso Software:**
    *   **Tarea:** Subir el reporte de la actividad realizada en clase sobre las fases del proceso SOF. Se recomienda leer el primer material de lectura en la plataforma para complementar o ajustar el trabajo.
    *   **Formato:** Un solo archivo PDF por equipo, con una portada que incluya los nombres de todos los integrantes.
    *   **Fecha Límite:** Sábado al final del día.
*   **ADA 1.2 - Guía de Lectura:**
    *   **Tarea:** De manera individual, leer el tercer material disponible en la plataforma ("El papel de la experimentación en Ing. de Software") y contestar la guía de preguntas proporcionada.
    *   **Fecha Límite:** Martes al final del día.
    *   **Discusión:** Los resultados se discutirán en la primera parte de la clase del próximo jueves.

