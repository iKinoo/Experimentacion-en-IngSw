|               |                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Fecha         | 22 de agosto de 2025                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Audio         | [OneDrive](https://alumnosuady-my.sharepoint.com/personal/a19203594_alumnos_uady_mx/_layouts/15/stream.aspx?id=%2Fpersonal%2Fa19203594%5Falumnos%5Fuady%5Fmx%2FDocuments%2FSemestres%2FSemestre%20VII%2FExperimentaci%C3%B3n%20en%20Ingenier%C3%ADa%20de%20Software%2FClases%2FGrabaciones%2Fexper%5Fvera%5F2025%2E08%2E22%2Em4a&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E6171a1d5%2D58cd%2D4ea9%2D81bb%2D0a7443662bbe) :lock: |
| Transcripción | [../raw/exper_vera_2025.08.22.mp3.txt](../raw/exper_vera_2025.08.22.mp3.txt)                                                                                                                                                                                                                                                                                                                                                                                 |

# Terminología y Conceptos Clave del Diseño Experimental

**Resumen**

La clase se dedicó a profundizar en la terminología fundamental del diseño experimental en el contexto de la ingeniería de software. Se partió de la definición de un experimento como el estudio de la variabilidad de una variable dependiente a través de la manipulación controlada de una variable independiente. Utilizando el ejemplo continuo de la revisión de código, se definieron y diferenciaron conceptos esenciales como: unidad experimental (el objeto de estudio, ej. el código), sujeto experimental (la persona que realiza la tarea, ej. el tester), variable dependiente (la métrica de resultado, ej. la eficacia), y variable independiente o factor (la condición que se manipula, ej. la técnica de revisión). Se hizo especial hincapié en la diferencia entre alternativas y tratamientos, explicando que un tratamiento es una combinación específica de los niveles de uno o más factores.

**Palabras Clave:**
Diseño Experimental, Factor, Tratamiento, Unidad Experimental, Sujeto Experimental, Variable Dependiente, Variable Independiente, Interacción, Parámetros.

## Reporte Detallado

La sesión se centró en desglosar los componentes de un experimento controlado, pasando del constructo teórico a su aplicación práctica. El objetivo es entender cada pieza para poder diseñar y analizar un experimento de manera rigurosa.

### De la Teoría a la Práctica

Se reiteró que un experimento parte de una teoría que postula una relación causa-efecto entre variables. Este constructo teórico se materializa en un experimento donde se deben definir operacionalmente dichas variables:

- **Variable Dependiente (o de Respuesta):** Debe traducirse en una métrica concreta, preferiblemente en una escala de razón que permita cálculos estadísticos robustos (media, desviación estándar, etc.).
- **Variable Independiente (o Factor):** Es la causa que se manipula. Sus valores pueden ser cualitativos (ej. Técnica A vs. Técnica B) o cuantitativos.

### Terminología Clave del Diseño Experimental

Se definieron los siguientes conceptos, utilizando el ejemplo de comparar dos técnicas de revisión de código:

1.  **Unidad Experimental (u Objeto Experimental):** Es la entidad sobre la cual se aplica el tratamiento y se observa la respuesta. Es la pieza fundamental que genera un valor representativo del resultado.

    - **Ejemplo:** El **código fuente** que es revisado por el tester. No es la persona, sino el objeto sobre el que se realiza la acción.

2.  **Sujeto Experimental:** Son las personas (o equipos) que ejecutan la tarea o aplican los tratamientos. En ingeniería de software, el sujeto es una fuente importante de variabilidad debido a factores como la experiencia, por lo que sus características deben ser controladas cuidadosamente.

    - **Ejemplo:** El **ingeniero de software** en su rol de tester que realiza la revisión.

3.  **Variable de Respuesta (o Dependiente):** Es la variable en la que se mide el efecto del factor. Es la salida del experimento y el foco del análisis.

    - **Ejemplo:** La **eficacia** (medida como el número de faltas detectadas) o la **eficiencia** (faltas detectadas por unidad de tiempo).

4.  **Variable Independiente (o Factor):** Es la variable que el investigador manipula intencionadamente para observar su efecto sobre la variable de respuesta.

    - **Ejemplo:** La **técnica de prueba** utilizada para la revisión de código.

5.  **Alternativas y Tratamientos:**

    - **Alternativas (o Niveles):** Son los diferentes valores que puede tomar un factor.
      - **Ejemplo:** Para el factor "técnica de prueba", las alternativas son "Técnica Tradicional" y "Técnica Innovadora".
    - **Tratamiento:** Es la condición experimental específica que se aplica a las unidades experimentales.
      - **Si hay un solo factor:** El tratamiento es sinónimo de la alternativa (ej. el tratamiento es "usar la Técnica Tradicional").
      - **Si hay múltiples factores:** El tratamiento es la **combinación** de los niveles de cada factor (ej. Técnica A + Tester Experto).

6.  **Parámetros:** Son características o variables del entorno experimental que se mantienen constantes (homogéneas) para que no influyan en los resultados y no se confundan con el efecto del factor estudiado.

    - **Ejemplo:** El nivel de _expertise_ de los sujetos (todos inexpertos), el lenguaje de programación del código, la complejidad del problema que resuelve el código.

7.  **Interacciones:** Ocurre cuando el efecto de un factor sobre la variable de respuesta depende del nivel de otro factor. Solo se puede estudiar en experimentos con dos o más factores.
    - **Ejemplo:** La técnica innovadora podría ser muy superior a la tradicional solo cuando la usan testers inexpertos, pero no mostrar diferencia significativa cuando la usan testers expertos.

### Preguntas y aclaraciones relevantes

- **¿Cuál es la diferencia entre "alternativa" y "tratamiento"?**
  El profesor aclaró esta duda de un estudiante. Son sinónimos cuando en el experimento solo se manipula **un factor**. Por ejemplo, si solo se compara la técnica A vs. la técnica B, "Técnica A" es tanto una alternativa como un tratamiento. Sin embargo, si se manipulan **dos o más factores** (ej. técnica y nivel de expertise), un **tratamiento** es una combinación específica de las alternativas de cada factor. Por ejemplo, un tratamiento sería "usar la Técnica A con un tester inexperto", y otro tratamiento sería "usar la Técnica B con un tester inexperto".

## Indicaciones Académicas

- **Próxima Sesión:** Se realizará una actividad práctica en clase. Se proporcionará un ejemplo de un experimento y los alumnos deberán identificar los elementos clave discutidos: sujeto, factor, tratamiento, unidad experimental, etc.
- **Nuevo Material:** Se subirá a la plataforma un cuarto material de lectura que contiene descripciones adicionales de los conceptos vistos en clase, con el fin de ofrecer diferentes perspectivas sobre la terminología.
