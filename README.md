# Análisis de Sentimiento y Tópicos en Posts de Reddit sobre Cambio Climático

## Descripción

Este proyecto tiene como objetivo analizar publicaciones de Reddit relacionadas con el cambio climático. Utilizamos técnicas de procesamiento de lenguaje natural (NLP) para realizar análisis de sentimiento, clustering de textos y análisis de tópicos.

## Tabla de Contenidos

* [Descripción](#descripcion)
* [Tabla de Contenidos](#tabla-de-contenidos)
* [Tecnologías Utilizadas](#tecnologias-utilizadas)
* [Instalación](#instalacion)
* [Uso](#uso)
* [Estructura del Proyecto](#estructura-del-proyecto)
* [Resultados Esperados](#resultados-esperados)
* [Información Adicional](#informacion-adicional)

## Tecnologías Utilizadas

* **Lenguaje de Programación:** Python
* **Bibliotecas:**
    * PRAW
    * Pandas
    * Spark
    * Transformers (Hugging Face)
    * Sentence Transformers
    * Scikit-learn

## Instalación

1. Clona este repositorio: `git clone https://github.com/TuNombreDeUsuario/NombreDeTuRepositorio.git`
2. Instala las dependencias: `pip install -r requirements.txt`

   Puedes generar el archivo `requirements.txt` con: `pip freeze > requirements.txt`

## Uso

1. Abre el notebook `nombre_de_tu_notebook.ipynb` en Google Colab.
2. Sigue las instrucciones dentro del notebook para ejecutar el código y obtener los resultados.

## Estructura del Proyecto

* `nombre_de_tu_notebook.ipynb`: Notebook principal con el código para extraer, procesar y analizar los posts de Reddit.
* `requirements.txt`: Archivo con las dependencias del proyecto.
* `data/`: (Opcional) Carpeta para guardar los datos descargados o procesados.
* `images/`: (Opcional) Carpeta para guardar imágenes o gráficos generados por el proyecto.

## Resultados Esperados

* **Posts Filtrados:** Se mostrarán los primeros 5 posts filtrados de Reddit.
* **Preprocesamiento:** Se mostrarán las palabras tokenizadas y limpias.
* **Análisis de Sentimiento:** Se mostrará el sentimiento asociado a cada texto.
* **Clustering:** Se mostrarán los clusters generados y ejemplos de textos en cada cluster.
* **Tópicos:** Se mostrarán los tópicos principales identificados con LDA.

## Información Adicional

* **Limitaciones:**
    * La API de Reddit tiene límites en la cantidad de requests que se pueden hacer en un tiempo determinado.
    * El análisis de sentimiento y tópicos puede verse afectado por el lenguaje utilizado en los posts y la complejidad del tema.
* **Mejoras Futuras:**
    * Explorar otros modelos de análisis de sentimiento y tópicos.
    * Utilizar técnicas de visualización para presentar los resultados de forma más clara.
    * Implementar un pipeline para automatizar el proceso de análisis.

## Autor

Paulina Peralta
