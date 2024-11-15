# Proyecto de Búsqueda y Clasificación de Páginas Web usando Embeddings de Texto
## Descripción
Este proyecto implementa un sistema de búsqueda y clasificación de páginas web basado en el contenido textual. Utiliza modelos de embeddings de texto para capturar la semántica de las palabras y realizar búsquedas en el corpus de páginas web. Se emplearon dos enfoques: un modelo Word2Vec entrenado desde cero y un modelo preentrenado de Sentence-BERT para comparar su desempeño en búsquedas contextuales.

## Dataset
El dataset utilizado es el archivo website_classification.csv, que incluye:

* website_url: URL de la página web.
* cleaned_website_text: Contenido textual limpiado extraído de la página web.
* category: Categoría de clasificación de la página web.
Este dataset contiene una muestra de sitios web clasificados en distintas categorías según el contenido textual, proporcionando una base para entrenar y evaluar modelos de embeddings.

## Modelos Utilizados
1.   Word2Vec
   El modelo Word2Vec fue entrenado desde cero en el corpus textual de las páginas web. Este modelo genera embeddings a nivel de palabra y permite medir similitudes entre términos específicos en el vocabulario del corpus.

* Ventaja: Captura relaciones entre palabras del corpus.
* Limitación: No maneja frases completas ni términos fuera del vocabulario.
2.   Sentence-BERT (SentenceTransformer 'all-MiniLM-L6-v2')
El modelo Sentence-BERT, preentrenado en grandes corpus de datos, genera embeddings a nivel de oración o frase, permitiendo búsquedas contextuales más robustas.

* Ventaja: Soporta búsquedas con oraciones completas y términos fuera del corpus.
* Limitación: Uso intensivo de recursos comparado con Word2Vec.
## Resultados y Conclusión
* Word2Vec es útil para análisis de relaciones entre palabras del corpus.
* Sentence-BERT es superior en búsquedas contextuales y consultas con frases completas o palabras desconocidas, proporcionando resultados más relevantes y precisos.

