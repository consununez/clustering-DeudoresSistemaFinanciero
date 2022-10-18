## Proyecto

Proyecto de análisis y modelado de datos de un dataset de la Central de Deudores del Sistema Financiero provisto por el BCRA, para la Diplomatura en 
Ciencia de Datos e Inteligencia Artificial dictada por FAMAF.
Trabajo realizado en tres notebook de Python: Preprocesamiento de datos; Análisis Exploratorio de datos; Modelado de datos. 


### Objetivos

A partir de la información obtenida de la Central de Deudores del BCRA, El objetivo es realizar un análisis exhaustivo de las personas que se 
encuentran dentro del dataset y poder realizar un clustering en base a los tipos de personas, al género en caso de la personas físicas, al monto de deuda, 
al tipo de entidad que otorgó el crédito y a si la deuda se encuentra en default o no. De esta manera buscamos conformar distintos grupos de deudores que 
permitan realizar comparaciones interesantes y útiles entre los mismos.


### Conclusiones

El objetivo era formar grupos que permitan identificar ciertas
particularidades entre los distintos tipos de deudores del dataset, que podrían ser útiles para
la toma de decisiones o nutrir otros procesos. Para ello se generó el modelo no
supervisado “K-means”, cuyo agrupamiento se realiza minimizando la suma de distancias
entre cada observación y el centroide de su clúster.
Para determinar el número de clusters óptimo a generar, se utilizó el método de Elbow, que
consiste en elegir aquel “k” (número de clusters) en donde la curva comienza a aplanarse, o
donde justamente se da el “codo”, por lo que agregar otro grupo no mejora sustancialmente
la distancia media intra-cluster.
Si bien se observan mejoras posibles con un número elevado de clusters, para un análisis inicial
se seleccionan 9 grupos para el modelado.
Luego de ejecutar el modelo, se observa que se formaron grupos bien heterogéneos y con
un interesante número de deudores para analizar.
Como se puede ver en el análisis de cluster, los mismos separan poblaciones con
potencialidad suficiente para enfocarse y direccionar estrategias comerciales, originación de
clientes, mejora de churn, etc.
