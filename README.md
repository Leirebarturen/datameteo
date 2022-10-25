# analisis_meteorologico

## ¿Qué es?
analisis_meteorologico es un paquete de Python que proporciona el acceso a datos meteorológicos para que el análisis de estos sea más rápido y sencillo. Después de definir cualquier ubicación, descarga datos metereológicos de temperatura, humedad, viento, precipitación y estado del cielo de las últimas 48 horas. Ofrece la posibilidad de mostrar los datos por pantalla como texto o por visualizaciones generando imágenes.     


## Principales características
La librería puede hacer las siguientes cosas:
* Muestra coordenadas de latitud y longitud de la ubicación introducida a través de Nominatim.
* Descarga de los datos en formato json.
* Temperatura de las últimas 24 horas en ºC.
* Humedad de las últimas 24 horas en g/m3.
* Rachas de viento de las últimas 48 horas en m/s.
* Precipitación de los últimos 48 minutos en l/m2.
* Tipos de estados de cielo.
* Posibilidad de mostrar gráficamnete los datos descargados mediante descriptivos numéricos, boxplots, gráficos de líneas y barras.

## Dónde conseguirlo
El código fuente está actualmente alojado en GitHub en: https://github.com/pandas-dev/pandas.
Los instaladores para la última versión publicada están disponibles en Python Package Index (PyPI).
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto" data-snippet-clipboard-copy-content="# or PyPI
pip install pandas"><pre><span class="pl-c"><span class="pl-c">#</span> or PyPI</span>
pip install pandas</pre></div>

## Dependencias
* <a href="[url](https://pypi.org/project/requests/)">requests - Realiza la petición de los datos a la API.</a>
* <a href="[url](https://geopy.readthedocs.io/en/stable/)">geopy - Ofrece as coordenadas de la ubicación introducida a través de la API Nominatim.</a>
* <a href="[url](https://pypi.org/project/pandas/)">pandas - Ofrece soporte y funciones para realizar descriptivos numéricos de los datos.</a>
* <a href="[url](https://matplotlib.org/)">matplotlib - Ofrece funciones para realizar gráficos de lineas de los datos. </a>
* <a href="[url](https://seaborn.pydata.org/)">seaborn - Ofrece funciones para realizar gráficos de líneas y barras de los datos.</a>

## Documentación
La documentación oficial está alojada en PyData.org: https://pandas.pydata.org/pandas-docs/stable
