## Descarga de los datos

Para el desarrollo del ejercicio hice uso de dos conjuntos de datos descargados de Datos Abiertos Colombia. 
El primer conjunto de datos corresponde a Predios Titulados a nivel Nacional, el cual contiene la sumatoria de predios urbanos, rurales, fiscales y privados, saneados y/o titulados a nivel nacional, el cual se muestra a continuación:

![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/7195121e-27c0-4b18-8cc8-87334f0cacd0)


## Limpieza de datos con Open Refine
Revisando el conjunto de datos, no se observan inconsistencias en la información, el dataset está muy limpio, no tiene datos en blanco ni información mal digitada. Sin embargo, con el fin de hacer uso de la herramienta (Open Refine) decidí separar y quitar las horas de las fechas de reporte y fechas del título quedando como se muestra a continuación:
•	Separando las columnas por delimitador “ “:
 ![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/f794df83-dae9-4ae1-ac66-ba2afc387142)

•	Conjunto de datos después de la separación y eliminación de las columnas:
 ![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/81a7838e-9ab8-4496-9aab-cf35003eed62)

Dataset 2

El segundo conjunto de datos corresponde a una Encuesta de Salud, derechos sexuales y reproductivos el cual se muestra a continuación:
 ![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/c6326dff-402c-448f-a06a-6a7340b93da2)

Al revisar el data set, se observa que tiene varios errores de digitación:

![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/36f53761-016a-4b83-88bf-60038a2538fa)
![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/f2e98cde-c3e9-4372-90b1-d12f2a516f8d)

Empiezo por ejecutar ‘Facet’ de la columna ‘Institución donde estudias’ y empiezo a generar clústeres, combinar y hacer re-cluster:
![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/a8e237ef-d7d3-481c-9696-134afbe49e17)

Generé re-clusters primero con el método de ‘Key Collision’, probando cada una de las funciones claves; con ‘Metaphone3’, ‘Levenshtein’ y por último con Vecinos cercanos.
Finalmente se puede observar que las elecciones en los datos pasaron de ser inicialmente 88 a 47 con la limpieza que se le hizo a la información:

![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/43fe6877-9435-456d-a217-708796a8c9b0)
![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/86ee2aa2-ef46-4acf-8879-8add9154ba26)

## Cruce de la información

Para llevar a cabo la integración de datos hice uso de otros 2 data sets, ya que los trabajados anteriormente no tenían nada en común. A continuación, se relaciona los data sets trabajados, los cuales igualmente fueron descargados de la base de datos wwww.datos.gov.co:

1.	Estadísticas en educación en Colombia
2.	Resultados nacionales saber 11 2019

## Limpieza en Power BI

![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/a8c6571c-d14d-4e11-807d-78cc69d9a90a)

![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/85281d44-ab38-4801-8004-f80f2f2fb3a7)

Estadístias![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/d7a73116-eada-469f-85af-9df0d68995c9)


![image](https://github.com/kathy-oviedo/Proyecto-Final-Bootcamp/assets/161944778/613d5c47-a9b5-4e0e-8f20-bb476e12d011)

Link del dashboard:

<iframe title="Proyecto_Final" width="600" height="373.5" src="https://app.powerbi.com/view?r=eyJrIjoiNmUxYjMxN2MtNjhhNi00ODdkLWFmNWQtMjUyYmQ5NzQ5NzkwIiwidCI6ImFjYTUxNjMxLTAwZmUtNDkwZC05MWFiLTE2M2VmODcyNjBlZSIsImMiOjR9" frameborder="0" allowFullScreen="true"></iframe>

https://app.powerbi.com/view?r=eyJrIjoiNmUxYjMxN2MtNjhhNi00ODdkLWFmNWQtMjUyYmQ5NzQ5NzkwIiwidCI6ImFjYTUxNjMxLTAwZmUtNDkwZC05MWFiLTE2M2VmODcyNjBlZSIsImMiOjR9


