Ejemplos
=============

Instalación/Uso
*******************
El código fuente está actualmente alojado en GitHub en: https://github.com/pandas-dev/pandas. Los instaladores para la última versión publicada están disponibles en Python Package Index (PyPI).
Para obtener instrucciones sobre cómo instalar, así como la documentación completa de, ``datameteo`` accede `aquí <https://github.com/Leirebarturen/datameteo>`_.

A continuación se mostra un ejemplo del uso de la librería:
**************************************************
.. code-block:: python
    
    """Este ejemplo demuestra el uso de la libreria ``datameteo``
    """

   import datameteo as dm

    # Se instancia la clase de generación de datos, especificando la ubicación y la API key para hacer la consulta
    datos_bilbao = dm.generar_datos(provincia = "Bilbao", api_key = "464aef7687e9220994fe3f4d43e9b22c")
    # Se descargan los datos meterológicos en formato json
    datos_bilbao.extraer_info()
    coord = datos_bilbao.coordenadas()
    print("Las coordenadas de Bilbao son %s" %(str(coord)))
    # Se muestra por pantalla la información general
    datos_bilbao.show()

    # Se instancia la clase de análisis de datos, especificando los parámetro para la descarga de datos y el direcotrio output para las figuras
    eda = dm.analizar_datos(provincia = "Bilbao", api_key = "464aef7687e9220994fe3f4d43e9b22c", out_path = "graf_met/")
    # Se muestran descriptivos básicos de todas las variables
    print(eda.descriptivos())
    # Se generan boxplots para cada una de las variables
    eda.boxplots()
    # Se genera la figura que meustra la evolución de la temperatua. Si no se especifica el parámetro variable, se genera una línea por cada varible
    eda.lineas(variable = "temperatura")
    # Se genera un gráfico de barras con el conteo de los estados del cielo
    eda.barras()