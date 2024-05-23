## Descarga de los datos

Primer Punto
1.	Dataset´s utilizados (Datos Abiertos Colombia | Datos Abiertos Colombia) al menos 2 (que no sean repetidos)
•	Aplicar Métodos de recolección y limpieza de datos (OpenRefine)
Dataset 1

Para el desarrollo del ejercicio hice uso de dos conjuntos de datos descargados de Datos Abiertos Colombia. 
El primer conjunto de datos corresponde a Predios Titulados a nivel Nacional, el cual contiene la sumatoria de predios urbanos, rurales, fiscales y privados, saneados y/o titulados a nivel nacional, el cual se muestra a continuación:

## Limpieza de datos con Open Refine
Revisando el conjunto de datos, no se observan inconsistencias en la información, el dataset está muy limpio, no tiene datos en blanco ni información mal digitada. Sin embargo, con el fin de hacer uso de la herramienta (Open Refine) decidí separar y quitar las horas de las fechas de reporte y fechas del título quedando como se muestra a continuación:
•	Separando las columnas por delimitador “ “:
 
•	Conjunto de datos después de la separación y eliminación de las columnas:
 
Dataset 2

El segundo conjunto de datos corresponde a una Encuesta de Salud, derechos sexuales y reproductivos el cual se muestra a continuación:
 
Al revisar el data set, se observa que tiene varios errores de digitación:
  

Empiezo por ejecutar ‘Facet’ de la columna ‘Institución donde estudias’ y empiezo a generar clústeres, combinar y hacer re-cluster:
 
Generé re-clusters primero con el método de ‘Key Collision’, probando cada una de las funciones claves; con ‘Metaphone3’, ‘Levenshtein’ y por último con Vecinos cercanos.
Finalmente se puede observar que las elecciones en los datos pasaron de ser inicialmente 88 a 47 con la limpieza que se le hizo a la información:
  
## Cruce de la información

 2.Utilizar las bibliotecas de Integración de datos de diversas fuentes y formatos en los Dataset´s trabajados en el punto anterior 
Realizar al menos un cruce entre dos Dataset´s (Pandas)
Para llevar a cabo la integración de datos hice uso de otros 2 data sets, ya que los trabajados anteriormente no tenían nada en común. A continuación, se relaciona los data sets trabajados:
1.	Estadísticas en educación en Colombia
2.	Resultados nacionales saber 11 2019
Procedí a realizar el cruce tras el cual dio como resultado la siguiente tabla, la cual unió los datos estadísticos educativos con los resultados de las pruebas saber pro con base en el departamento:
 
Tercer y cuarto Punto
 3. Utilizar las bibliotecas de Análisis de series temporales 
Realizar al menos 3 gráficos de la información contenida en los Dataset´s anteriores utilizando las bibliotecas vistas.
Haciendo uso de la data set de “Encuesta de Salud, derechos sexuales y reproductivos” generé este gráfico:
 
Conclusiones:
•	En el gráfico se puede observar que la mayoría de los encuestados no tiene información sobre embarazos adolescentes en su comunidad.
•	Aproximadamente el 22% cree que solo uno de cada diez adolescentes ha experimentado un embarazo.
•	Un 30% de los encuestados cree que más de dos de sus compañeros adolescentes han experimentado un embarazo.

Luego, se hizo uso de otros de los data sets trabajados, en este caso el de tasas de Estadísticas en educación en Colombiama sobre el cual se generaron los siguientes gráficos:

 
Conclusiones:

•	En el gráfico se puede observar que Bogotá para el año 2019 tuvo una tasa de matrícula consistentemente mayor que la de Antioquia.
•	De igual manera también se puede observar que, antes del 2018, Bogotá tenía tasas de matrícula muy bajas respecto a Antioquia y que de alguna manera esto mejoró a partir de ese año, sería importante entrar a revisar, que causó ese aumento. 
•	Para el año 2022 se ve que ambos lugares, presentan una tasa de matriculación muy cercana.
 
Conclusiones:
•	Existe una correlación positiva entre la tasa de matrícula y la cobertura neta en Bogotá. Esto significa que a medida que aumenta la cobertura neta también aumenta la tasa de matrícula. Esto indica que existe una relación estrecha entre las dos variables.
•	La tendencia es lineal, lo que significa que la relación entre las dos variables es constante.





