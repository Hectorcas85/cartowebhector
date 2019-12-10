## Cuál es el problema a tratar?



## Por qué la publicación de servicios OGC puede ayudar a resolverlo?


## Qué servicios propone para la solución de su problema? WMS? WMTS? WFS? Por qué ?

## Descripción de los datos seleccionados (Origen, descripción, características especiales, atributos, url para descarga)

## Descripción del procesamiento realizado con postgis (Incluir los sqls)

## Descripción de la forma en que creó la simbología (incluir los sld's y css)

## Nombres de las tablas creadas en postgis

* u2_departamentos
* u2_Parques_NNC

## Nombres de las capas y estilos publicadas en geoserver.
## Url de la previsualización del grupo de capas en Geoserver
## Pantallazos con la forma en que los usuarios pueden consultar su geoservicio a través de QGIS
## Ventajas / desventajas / dificultades encontradas durante el proceso

En la capa inicial se tenia un total de 6599 registros, pero solo se logro subir 3000 registros
el error que salio fue el siguiente.

Ha ocurrido un error mientras se ejecutaba el código de Python:
db_manager.db_plugins.plugin.ConnectionError: server closed the connection unexpectedly This probably means the server terminated abnormally before or while processing the request.
Traceback (most recent call last):
File "C:/PROGRA1/QGIS31.4/apps/qgis-ltr/./python/plugins\db_manager\db_plugins\connector.py", line 86, in _execute
cursor.execute(sql)
psycopg2.OperationalError: server closed the connection unexpectedly
This probably means the server terminated abnormally
before or while processing the request.
During handling of the above exception, another exception occurred:
Traceback (most recent call last):
File "C:/PROGRA1/QGIS31.4/apps/qgis-ltr/./python/plugins\db_manager\dlg_import_vector.py", line 371, in accept
self.db.connector.createSpatialIndex((schema, table), geom)
File "C:/PROGRA1/QGIS31.4/apps/qgis-ltr/./python/plugins\db_manager\db_plugins\postgis\connector.py", line 970, in createSpatialIndex
self._execute_and_commit(sql)
File "C:/PROGRA1/QGIS31.4/apps/qgis-ltr/./python/plugins\db_manager\db_plugins\connector.py", line 100, in _execute_and_commit
self._execute(None, sql)
File "C:/PROGRA1/QGIS31.4/apps/qgis-ltr/./python/plugins\db_manager\db_plugins\connector.py", line 89, in _execute
raise ConnectionError(e)
db_manager.db_plugins.plugin.ConnectionError: server closed the connection unexpectedly
This probably means the server terminated abnormally
before or while processing the request.
Versión de Python: 3.7.0 (v3.7.0:1bf9cc5093, Jun 27 2018, 04:59:51) [MSC v.1914 64 bit (AMD64)]
Versión de QGIS: 3.4.13-Madeira Madeira, 64ad560274
Ruta de Python:
C:/PROGRA1/QGIS31.4/apps/qgis-ltr/./python
C:/Users/LENOVO/AppData/Roaming/QGIS/QGIS3\profiles\default/python
C:/Users/LENOVO/AppData/Roaming/QGIS/QGIS3\profiles\default/python/plugins
C:/PROGRA1/QGIS31.4/apps/qgis-ltr/./python/plugins
C:\Program Files\Hexagon\ERDAS IMAGINE 2015\usr\lib\Win32Release\python
C:\Program Files\QGIS 3.4\bin\python37.zip
C:\PROGRA1\QGIS31.4\apps\Python37\DLLs
C:\PROGRA1\QGIS31.4\apps\Python37\lib
C:\Program Files\QGIS 3.4\bin
C:\PROGRA1\QGIS31.4\apps\Python37
C:\PROGRA1\QGIS31.4\apps\Python37\lib\site-packages
C:\PROGRA1\QGIS31.4\apps\Python37\lib\site-packages\win32
C:\PROGRA1\QGIS31.4\apps\Python37\lib\site-packages\win32\lib
C:\PROGRA1\QGIS31.4\apps\Python37\lib\site-packages\Pythonwin
C:/Users/LENOVO/AppData/Roaming/QGIS/QGIS3\profiles\default/python
C:/Users/LENOVO/AppData/Roaming/QGIS/QGIS3\profiles\default/python/plugins\qgis2web
C:\Users\LENOVO\AppData\Roaming\QGIS\QGIS3\profiles\default\python\plugins
