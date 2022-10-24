# Inmersión en la Streaming Wars: Un EDA enfocado en el negocio de las plataformas de streaming

Este EDA ha sido realizado por César Herreros Castillo para el bootcamp The Bridge en Madrid. En este, he desarollado la siguiente pregunta:
* ¿Qué tipo de películas producir en cuanto a género y presupuesto? ¿Cómo sería la distribución del contenido en la plataforma?

La hipótesis de partida es la siguiente:
* Las películas a producir serán aquellas cuyos géneros sean más rentables producir y estén mejor valorados por el público.
* En cuanto a la distribución del contenido en la plataforma, se debe seguir la plataforma Netflix como referencia a tener en cuenta, puesto que es la principal plataforma del mercado.

El repositorio cuenta con dos carpetas. En src.data se encuentran tanto las bases de datos utilizadas como los gráficos realizados, mientras que en src.notebooks están los notebooks donde he realizado todo el trabajo. Estructurado de la siguiente manera:

## 1. Limpieza de datos
* Limpieza de las principales variables a utilizar, así como creación de nuevos dataframes.

## 2. Análisis financiero
En este notebook se han llevado los análisis relacionados con las finanzas y el mundo del cine intentando dar respuesta las siguientes preguntas:
* ¿Qué generos son los costosos de producir? ¿Cuáles son más rentables?
* ¿Existe una relación entre el presupuesto y el beneficio obtenido?
* ¿Cuál es el presupuesto óptimo para producir una película rentable?

## 3. Popularidad
* ¿Qué géneros son los más populares?
* ¿Existe correlación entre popularidad y beneficio?

## 4. Análisis de Netflix
Desarrollar una plataforma de streaming requiere, principalmente, de productos que no son propios de la empresa, sino que adquieren los derechos de innumerables películas y series.

En este notebook, tomando de referencia a Netflix, busco dar respuestas a:
* Proporción de géneros
* Proporción de películas y series
* Proporción de rangos de edad
* Proporción de producciones por país de origen
* Proporción de producciones en función del año de la producción

## 5. Reparto
Para obtener los artistas más populares del momento he realizado webscrapping en la lista de los 50 artistas más populares del momento en la web de IMDb. He recogido nombre, sexo, papel más actual y breve descripción de la persona.

El objetivo es crear un dataframe con los artistas del momento
