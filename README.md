# tfm-analisi_corpus_aranes
Trabajo de final de máster de ciencia de datos de la UOC, titulado "Análisis del uso contemporáneo del aranés mediante técnicas de procesamiento de lenguaje natural en u contexto de recursos limintados".


# Análisis Computacional y Lingüístico de un Corpus en Aranés 🏔️📊

Este repositorio contiene todo el código fuente y los flujos de procesamiento de datos.

Los origenes de datos no se incluyen en este repositorio.

Este proyecto implementa un pipeline con los siguientes pasos:
  - Extracción de texto en bruto.
  - Limpieza y estructuración de los datos.
  - Procesamiento y análisis sintáctico.
  - Análisis semántico.


## 📂 Estructura del Proyecto

El repositorio está organizado de forma modular, separando los datos, el código de ejecución y los artefactos resultantes:

* **`data/`**: Contiene los textos originales, el lexicón base y los diccionarios morfológicos.
* **`corpus_json/`**: Directorio donde se almacenan los archivos `.jsonl` resultantes de las diferentes fases de limpieza, unificación y anotación sintáctica.
* **`scripts/`**: Corazón del proyecto, dividido en dos módulos funcionales:
  * `create_json/`: Scripts dedicados al preprocesamiento, normalización léxica y etiquetado morfosintáctico (POS Tagging).
  * `analysis/`: Suite de algoritmos cuantitativos, estadística léxica y Machine Learning.
* **`resultados_corpus/`**: Carpeta de salida automatizada para gráficas de lingüística computacional (Ley de Heaps, nubes de palabras, TF-IDF).
* **`modelo/`**: Directorio destinado al almacenamiento de los vectores densos locales (FastText), gráficas de clustering semántico (SBERT + UMAP) y datos NER.

---

## ⚙️ Requisitos e Instalación

Para reproducir los experimentos y el análisis de este TFM, se requiere Python 3.9 o superior. 

**1. Clonar el repositorio y preparar el entorno:**
```bash
git clone [https://github.com/TU_USUARIO/TU_REPOSITORIO.git](https://github.com/TU_USUARIO/TU_REPOSITORIO.git)
cd TU_REPOSITORIO
python -m venv .venv
# Activar entorno virtual (Windows)
.venv\Scripts\activate
# Activar entorno virtual (Mac/Linux)
source .venv/bin/activate
