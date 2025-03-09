# Procesamiento del lenguaje natural para el análisis de sentimientos y tópicos sobre cambios medioambientales de la plataforma Reddit

![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)
![PySpark](https://img.shields.io/badge/PySpark-3.1+-orange.svg)
![HuggingFace](https://img.shields.io/badge/HuggingFace-Transformers-yellow.svg)
![NLTK](https://img.shields.io/badge/NLTK-3.6+-green.svg)
![License](https://img.shields.io/badge/License-MIT-purple.svg)

## Descripción

Este proyecto implementa un sistema integral para analizar contenido sobre cambio climático en la plataforma Reddit. Mediante técnicas avanzadas de procesamiento de lenguaje natural (NLP), análisis de sentimiento, clustering semántico y modelado de tópicos, se examina cómo las comunidades digitales expresan percepciones, preocupaciones y conocimientos sobre la crisis climática.

El sistema extrae datos de subreddits relevantes, procesa la información textual, identifica patrones temáticos y genera visualizaciones interpretables junto con un informe científico estructurado.

## Características principales

- 🤖 **Extracción automatizada** de posts de múltiples subreddits relacionados con el clima
- 📊 **Análisis multi-método de sentimiento** combinando VADER y modelos transformers
- 🔍 **Clustering semántico** basado en embeddings de SentenceTransformer
- 📚 **Modelado de tópicos** mediante Latent Dirichlet Allocation (LDA)
- 👥 **Reconocimiento de entidades nombradas** para identificar actores relevantes
- 📈 **Visualizaciones interactivas** de resultados mediante Matplotlib, Seaborn y Plotly
- 📑 **Generación automática** de informes científicos en formato HTML

## Tecnologías utilizadas

- **PRAW**: Interacción con la API de Reddit
- **PySpark**: Procesamiento distribuido de texto
- **Transformers**: Modelos pre-entrenados para análisis de sentimiento
- **SentenceTransformer**: Generación de embeddings semánticos
- **spaCy**: Reconocimiento de entidades nombradas
- **NLTK**: Análisis lingüístico y de sentimiento
- **scikit-learn**: Clustering y modelado de tópicos
- **Matplotlib/Seaborn/Plotly**: Visualización de datos

## Ejemplos de visualizaciones

El proyecto genera diversas visualizaciones para analizar patrones en las conversaciones sobre cambio climático:

- Distribución de sentimiento entre diferentes subreddits
- Nubes de palabras categorizadas por sentimiento
- Visualización de clusters temáticos mediante t-SNE
- Distribución y análisis de tópicos descubiertos
- Entidades nombradas más frecuentes
- Análisis temporal de volumen y sentimiento

## Instalación y uso

### Prerrequisitos

- Python 3.7+
- PySpark
- Acceso a la API de Reddit (credenciales)

### Configuración

1. Clona este repositorio:
```bash
git clone https://github.com/PaulinaIA/reddit-climate-analysis.git
cd reddit-climate-analysis
```

2. Instala las dependencias:
```bash
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```

3. Configura tus credenciales de Reddit:
```python
# Edita el archivo config.py o establece variables de entorno
CLIENT_ID = "tu_client_id"
CLIENT_SECRET = "tu_client_secret"
USER_AGENT = "nombre_de_tu_aplicacion"
```

### Ejecución

```python
# Ejecutar análisis completo
python reddit_climate_analysis.py

# Para ejecutar con opciones personalizadas
python reddit_climate_analysis.py --subreddits climatechange,environment --time_period 60 --post_limit 500
```

### Uso en Google Colab

También puedes ejecutar este análisis en Google Colab. El notebook `Reddit_Climate_Analysis.ipynb` está adaptado para ese entorno, con optimizaciones para manejar las limitaciones de memoria y procesamiento.

## Estructura del proyecto

```
reddit-climate-analysis/
│
├── reddit_climate_analysis.py      # Script principal
├── Reddit_Climate_Analysis.ipynb   # Notebook para Google Colab
├── requirements.txt                # Dependencias
├── config.py                       # Configuración y credenciales
│
├── data/                           # Directorio para datos
│   └── climate_terms.json          # Términos relacionados con cambio climático
│
├── resultados/                     # Directorio para resultados
│   ├── visualizaciones/            # Visualizaciones generadas
│   ├── cluster_analysis.json       # Análisis de clusters
│   ├── topics_info.json            # Información de tópicos
│   └── climate_analysis_report.html # Informe científico
│
└── utils/                          # Utilidades y módulos auxiliares
    ├── nlp_utils.py                # Funciones de procesamiento de lenguaje
    ├── visualization.py            # Funciones para visualizaciones
    └── report_generator.py         # Generador de informes
```

## Resultados e insights

El análisis genera un informe científico completo (`climate_analysis_report.html`) que incluye:

- Distribuciones de sentimiento y su variación entre comunidades
- Patrones temáticos identificados mediante clustering
- Tópicos latentes descubiertos con LDA
- Análisis de entidades y actores prominentes
- Evolución temporal del contenido
- Conclusiones y limitaciones metodológicas

## Metodología

El proyecto sigue un flujo de trabajo estructurado:

1. **Recolección de datos**: Extracción de posts relevantes mediante la API de Reddit
2. **Preprocesamiento**: Limpieza, tokenización y vectorización de textos
3. **Análisis de sentimiento**: Combinación de métodos léxicos (VADER) y basados en transformers
4. **Clustering**: Agrupamiento semántico basado en embeddings
5. **Modelado de tópicos**: Descubrimiento de temas latentes mediante LDA
6. **Análisis de entidades**: Identificación de organizaciones, personas y lugares mencionados
7. **Visualización**: Generación de gráficos interpretativos
8. **Reporte**: Compilación de hallazgos en un informe estructurado

## Autora

**Paulina Maria Peralta Escurra**  
- Email: pauliperalta97@gmail.com
- GitHub: [PaulinaIA](https://github.com/PaulinaIA)

## Licencia

Este proyecto está licenciado bajo la Licencia MIT - vea el archivo [LICENSE](LICENSE) para más detalles.

## 🙏 Agradecimientos

- Agradecimiento a la comunidad de Reddit por proporcionar un espacio para conversaciones sobre cambio climático
- Librerías de código abierto que hicieron posible este análisis
