|               |                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Fecha         | 05 de septiembre de 2025                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Audio         | [OneDrive](https://alumnosuady-my.sharepoint.com/personal/a19203594_alumnos_uady_mx/_layouts/15/stream.aspx?id=%2Fpersonal%2Fa19203594%5Falumnos%5Fuady%5Fmx%2FDocuments%2FSemestres%2FSemestre%20VII%2FExperimentaci%C3%B3n%20en%20Ingenier%C3%ADa%20de%20Software%2FClases%2FGrabaciones%2Fexper%5Fvera%5F2025%2E09%2E05%2Em4a&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E1db3eb9d%2Dcef9%2D40fd%2Daa90%2D9c8e473d5b34) :lock: |
| Transcripción | [../raw/exper_vera_2025.09.05.m4a.txt](../raw/exper_vera_2025.09.05.m4a.txt)                                                                                                                                                                                                                                                                                                                                                                                  |

# Fases del Proceso Experimental y Diseños con Múltiples Factores

**Resumen**

La clase se centró en consolidar los principios del diseño experimental y en presentar el proceso estructurado para llevar a cabo un experimento en ingeniería de software. Se inició con un repaso interactivo de los principios de **repetición**, **aleatorización**, **bloqueo** y **factorización**. Posteriormente, se detalló el proceso experimental a través de una serie de pasos genéricos y un modelo formal de cuatro fases: **Definición, Diseño, Ejecución y Análisis**. Se hizo hincapié en la elección del diseño experimental, ilustrando con ejemplos la diferencia entre diseños con muestras independientes y muestras dependientes (pareadas). Finalmente, se introdujo una nueva actividad práctica que consistirá en analizar un artículo de investigación sobre "Pair Programming" para identificar cómo se aplican estas fases en un estudio real.

**Palabras Clave:** 
Proceso Experimental, Diseño Experimental, Repetición, Aleatorización, Bloqueo, Factorización, Muestras Independientes, Muestras Pareadas, Pair Programming.

## Reporte Detallado

La sesión profundizó en la metodología para la planificación y ejecución de experimentos controlados, pasando de los principios teóricos a un marco de trabajo estructurado.

### 1. Repaso de Principios del Diseño Experimental

Se revisaron los cuatro principios fundamentales discutidos en la clase anterior:

*   **Aleatorización:** Asignar al azar los sujetos a los tratamientos para distribuir de manera equitativa el efecto de variables no controladas (ej. capacidad cognitiva, motivación), evitando así sesgos.
*   **Repetición:** Realizar múltiples "experimentos unitarios", es decir, tener varios sujetos por cada tratamiento. Esto permite una mejor estimación del error experimental y aumenta la fiabilidad de los resultados.
*   **Bloqueo:** Técnica utilizada cuando existe un factor conocido que influye en la respuesta (ej. nivel de expertise), pero que no es el foco principal del estudio. Se crean "bloques" homogéneos (ej. un grupo de expertos y un grupo de inexpertos) y se asignan los tratamientos aleatoriamente dentro de cada bloque para controlar esa fuente de variabilidad.
*   **Factorización (Diseño Factorial):** Estrategia que se emplea cuando se desea estudiar el efecto de dos o más factores simultáneamente, así como la posible **interacción** entre ellos. Es más eficiente que estudiar cada factor por separado.

### 2. Fases del Proceso Experimental

Se presentó un modelo estructurado y reconocido para llevar a cabo un experimento, dividido en cuatro fases principales, mostrando la evolución de las propuestas de autores como Basili, Wohlin y Juristo.

![Diagrama del proceso experimental y tabla comparando las fases según diferentes autores.](/recursos/exper_vera_2025.09.05/el_proceso_experimental.jpg)

1.  **Fase de Definición y Objetivo:**
    *   Se establece la hipótesis de investigación y se traduce a hipótesis estadísticas.
    *   Se identifican claramente el factor (variable independiente) con sus alternativas, y la variable de respuesta (dependiente) con su métrica e indicador estadístico (ej. la media).

2.  **Fase de Diseño y Planificación:**
    *   Se organiza cómo se llevará a cabo el experimento. Implica la preparación de materiales (ej. el código a revisar, inyectándole faltas intencionadamente), la caracterización y selección de los sujetos, y la elección del diseño experimental.
    *   Se ilustró la diferencia entre dos tipos de diseño:
        *   **Diseño con Muestras Independientes:** Se utilizan sujetos diferentes para cada tratamiento. Ejemplo: 10 estudiantes, 5 son asignados a la Técnica A y los otros 5 a la Técnica B.
        *   **Diseño con Muestras Dependientes (o Pareadas):** Los mismos sujetos son expuestos a todos los tratamientos. Esto es común cuando el número de sujetos es limitado (ej. equipos de desarrollo). Ejemplo: 2 equipos realizan múltiples proyectos, aplicando aleatoriamente las técnicas A y B en diferentes proyectos (comparables entre sí para evitar el efecto de aprendizaje).
    
    ![Ilustración de dos diseños experimentales: muestras independientes y dependientes.](/recursos/exper_vera_2025.09.05/diseños_experimentales.jpg)

3.  **Fase de Ejecución:**
    *   Se lleva a cabo el experimento siguiendo el plan.
    *   Implica dar instrucciones o capacitación a los sujetos, ejecutar la tarea en un entorno controlado y recolectar los datos. Se destacó que la recolección de métricas puede requerir un post-procesamiento por parte del investigador (ej. evaluar la calidad de un diagrama para asignarle un puntaje).

4.  **Fase de Análisis e Interpretación:**
    *   Se analizan los datos recolectados mediante estadística descriptiva (resumir y visualizar) e inferencial (probar hipótesis).
    *   Se contrastan las hipótesis, se aceptan o rechazan, se generan conclusiones basadas en la evidencia y se proponen mejoras o trabajos futuros.

### 3. Aplicación Práctica: Análisis de un Artículo sobre Pair Programming

Para la siguiente actividad, se introdujo un artículo de investigación que compara la programación individual contra la programación en pareja. Se guio a los estudiantes a través de la estructura del artículo para que pudieran identificar preliminarmente:
*   **Factor:** Estilo de programación (Individual vs. Pareja).
*   **Variables de Respuesta:** Duración y Esfuerzo de la tarea.
*   **Diseño:** Se menciona un diseño de "Cuadrado Latino" con variables de bloqueo.
*   **Análisis y Conclusión:** Se observó cómo los autores interpretan el valor p para concluir que existen diferencias significativas.

![Slide que muestra la tabla de resultados del análisis del artículo de ejemplo.](/recursos/exper_vera_2025.09.05/análisis.jpg)

### Preguntas y Aclaraciones Relevantes

*   **¿Qué es la repetición en un experimento?**
    Se aclaró que la **repetición** no es que un mismo sujeto haga la misma tarea varias veces (lo cual introduce un efecto de aprendizaje), sino que **múltiples sujetos** realicen la tarea bajo las mismas condiciones. A mayor número de sujetos (repeticiones), más robusto es el experimento.
*   **¿Cuál es la diferencia entre Bloqueo y Factorización?**
    Ambos se usan cuando hay más de un factor influyente. Se usa **Bloqueo** cuando se quiere controlar el efecto de un factor conocido pero que **no se quiere estudiar** (se trata como "ruido" a eliminar). Se usa **Factorización** cuando se quiere **estudiar el efecto de todos los factores y su interacción**.

## Indicaciones Académicas

*   **Próxima Actividad de Aprendizaje:**
    *   **Tarea:** Leer y analizar el artículo proporcionado sobre "Pair Programming".
    *   **Objetivo:** Identificar y citar las secciones del artículo que correspondan a cada una de las cuatro fases del proceso experimental: Definición, Diseño, Ejecución y Análisis.
    *   **Fecha de entrega:** Se indicará en la plataforma (posiblemente para el miércoles).
*   


### Anexos Adicionales

![text](/recursos/exper_vera_2025.09.05/aplicación_del_proceso_de_experimentación.jpg)
![text](/recursos/exper_vera_2025.09.05/conclusiones.jpg)