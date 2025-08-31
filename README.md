# 📖 Expermentación en Ingeniería de Sofware: *Smart-AI Notes*

Este repositorio centraliza todas las transcripciones y resúmenes de las clases del curso de **Experimentación en Ingeniería de Software**.

> Disclaimer: Los archivos de audio son privados, solo accesible mediante permiso.

##  <img src="assets/Music Play.gif"  width="25"/> Últimas Clases

- [Teoría de la Medición y Escalas de Medición en Ingeniería de Software](resúmenes/exper_vera_2025.08.29.md) $\cdot$ *29/08*
- [Análisis Práctico de un Experimento: Factor Humano y Procesos de Software](resúmenes/exper_vera_2025.08.28.md) $\cdot$ *28/08*
- [Terminología y Conceptos Clave del Diseño Experimental](resúmenes/exper_vera_2025.08.22.md) $\cdot$ *22/08*
- [Métodos de Investigación Empírica en Ingeniería de Software](resúmenes/exper_vera_2025.08.21.md) $\cdot$ *21/08*

## 📂 Estructura de Carpetas

El contenido está organizado de la siguiente manera para facilitar el acceso y la consulta:

- **[/raw](./raw)**: Contiene las transcripciones automáticas y en bruto de las grabaciones de cada clase. Estos archivos (`.txt`) sirven como la fuente primaria y sin procesar del contenido.

- **[/resúmenes](./resúmenes)**: Aquí se guardan los resúmenes curados y formateados en Markdown (`.md`) de cada clase. Son la versión refinada, corregida y fácil de leer, ideal para repasos rápidos.

- **[/templates](./templates)**: Almacena las plantillas utilizadas para estandarizar la creación de los resúmenes y otros documentos del repositorio.

- **[/recursos](./recursos)**: Destinado a guardar recursos adicionales mencionados en clase, como diapositivas, enlaces a artículos, o lecturas complementarias.

## 🚀 Flujo de Trabajo

El proceso para generar el material de estudio es el siguiente:

1.  **Grabación:** Se graba el audio de la clase.
2.  **Transcripción:** El audio se procesa usando [WhisperX]([https://](https://github.com/m-bain/whisperX)) para generar un archivo de texto base en la carpeta `raw/`.
3.  **Elaboración de Resumen:** Utilizando la plantilla de `templates/template.md`, se revisa la transcripción en bruto para crear un resumen detallado y corregido con ayuda de [Gemini 2.5 Pro]([https://](https://aistudio.google.com/)) Gemini 2.5 Pro, el cual se almacena en `resúmenes/`.

---
