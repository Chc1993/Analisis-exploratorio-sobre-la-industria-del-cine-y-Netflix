# Inmersión en la Streaming Wars: Un EDA enfocado en el negocio de las plataformas de streaming

![human_afterall](https://user-images.githubusercontent.com/98810076/205484007-267e8366-eb0d-4634-bb50-c865c9d46077.png) 

Este EDA ha sido realizado por César Herreros Castillo para el bootcamp The Bridge en Madrid. En este, he partido del supuesto en el cual se va a desarrollar una nueva plataforma de streaming (con contenido propio). He planteado la siguiente pregunta:
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
![output](https://user-images.githubusercontent.com/98810076/214526174-81b089d3-8166-4a47-9a38-7512273aae16.png)

![output](https://user-images.githubusercontent.com/98810076/214526562-44336f8b-a9a2-481f-b818-0dd28bde1a1d.png)
![output](https://user-images.githubusercontent.com/98810076/214527021-3bb32700-691b-4bc9-83a5-9b5e110ce90d.png)


* ¿Existe una relación entre el presupuesto y el beneficio obtenido?
Correlación del 67,25% que se dispara a partir de los 80 millones de presupuesto.
![output](https://user-images.githubusercontent.com/98810076/214526804-65ef86bc-69b5-4bc4-b05f-d8e57d860f7a.png)

Correlación del 45,15% que se estanca a partir de los 80 millones brutos (marginal) de presupuesto.
![output](https://user-images.githubusercontent.com/98810076/214527327-e9a5eb7f-0849-451d-b2e8-fb9889af1041.png)

* ¿Cuál es el presupuesto óptimo para producir una película rentable?
En función de los resultados obtenidos, no sería producente una presupuesto superior a 80 millones.

## 3. Popularidad
* ¿Qué géneros son los más populares?
![output](https://user-images.githubusercontent.com/98810076/214527616-e2de1e88-d86c-4a1b-924a-963539a2fd06.png)

* ¿Existe correlación entre popularidad y beneficio?
La correlación es del 19,35%. Luego no hay correlación entre la popularidad (según IMdB) y el beneficio obtenido.

## 4. Análisis de Netflix
Desarrollar una plataforma de streaming requiere, principalmente, de productos que no son propios de la empresa, sino que adquieren los derechos de innumerables películas y series.

En este notebook, tomando de referencia a Netflix, busco conocer la:
* Proporción de géneros
![output](https://user-images.githubusercontent.com/98810076/214529171-0c0bb805-7f83-4e7e-b976-0e6d35eb1a43.png)
* Proporción de películas y series
![output](https://user-images.githubusercontent.com/98810076/214529026-9be8e3af-706b-47b9-ac31-c89a2af68ff5.png)
* Proporción de rangos de edad
![output](https://user-images.githubusercontent.com/98810076/214529080-5730464f-fe31-4d56-9114-93701a4ebe37.png)
* Proporción de producciones por país de origen
![output](https://user-images.githubusercontent.com/98810076/214529240-82a176f4-becf-4c88-846f-2699f6dbf9ab.png)
* Proporción de producciones en función del año de la producción
El catálogo es principalmente actual. El contenido anterior a 2010 es más escaso,  son outliers.En este caso podemos encontrar peliculas famosas o de culto: Taxi Driver o Deliverance
![output](https://user-images.githubusercontent.com/98810076/214528593-152915db-742e-400c-b539-2a49c51b1937.png)

## 5. Reparto
Para obtener los artistas más populares del momento he realizado webscrapping en la lista de los 50 artistas más populares del momento en la web de IMDb. He recogido nombre, sexo, papel más actual y breve descripción de la persona.

El objetivo es crear una tabla con los artistas del momento. (disponible en el repositorio en formato PDF)


Librerías utilizadas: Numpy, Pandas, Matplotlib, Seaborn, BeautifulSoup
