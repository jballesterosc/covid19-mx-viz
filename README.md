# covid19-mx-viz
En este repositorio encontrarás el código para hacer  ***visualizaciones básicas*** en Python del COVID-19 para cualquier entidad de México, a partir de las series de tiempo publicadas diariamente por Mario Jiménez en [*covid19-mx-time-series*](https://github.com/mariorz/covid19-mx-time-series)<sup>1</sup>

#¿Qué necesitas?
Previo a visualizar los datos de la sección *indicadores*, deberás tener instalado Python y los paquetes `pandas` y `matplotlib`. En mi caso, fue vía el [instalador de paquetes *pip*](https://pypi.org/project/pip/). 

Puedes replicarlo en tu *terminal de la siguiente manera:
````
pip install pandas
pip install matplotlib
``````
## Para correr el código
Lo más eficiente para mí fue trabajarlo desde [*Jupyter Notebooks*](https://jupyter.org), sobre todo, por lo fácil de seleccionar celdas específicas y procurar *atender un problema a la vez*. Para mí, insisto, que estoy aprendiendo a trabajar con datos en Python, fue de mucha ayuda para entender la lógica de cada linea de código. 

# A visualizar
 En la siguiente tabla encontrarás cada uno de los indicadores que podrás visualizar y el nombre de su archivo dentro de este repositorio. Para saber para qué funciona cada línea y cómo interacturar con el código,  encontrarás comentarios en todos los archivos —los reconoceras por inciar con: `#`—. Por ejemplo:

``````
# Este es un comentario. Las siguiente dos líneas son código interpretable.
import pandas as pd
import matplotlib as plt
``````

## Indicadores y código
Los archivos de la tabla y sus visualizaciones, están disponibles en la carpeta *notebooks* de este repositorio. 

| Nombre del archivo | Descripción |  
| ------------------------------------ | -------------------------------------------  |
| positivos_registro.ipynb | Casos positivos acumulados por fecha de registro | 
| positivos_sintomas.ipynb | Casos positivos acumulados por fecha de inicio de síntomas | 
| hospitalizados_admision.ipynb | Casos hospitalizados confirmados por fecha de admisión |
| hospitalizados_sintomas.ipynb | Casos hospitalizados confirmados por fecha de inicio de síntomas
| sospechosos_registro.ipynb | Casos sospechosos por fecha de registro |
| sospechosos_sintomas.ipynb | Casos sospechosos por fecha de inicio de síntomas |
| defunciones_registro.ipynb | Defunciones de casos positivos acumulados por fecha de registro | 
| defunciones_admision.ipynb | Defunciones de casos positivos acumulados  por fecha de admisión |
| defunciones_fecha.ipynb | Defunciones de casos positivos acumulados por fecha de defunción |
| defunciones_sintomas.ipynb | Defunciones de casos positivos acumulados por fecha de inicio de síntomas |

Cada archivo, una vez instalado *Python* y *Jupyter Notebooks*, podrás verlo en este último de la siguiente manera: 

<img src="https://i.imgur.com/jrMlYxa.png" width="700">

Al terminar de correr el código, se guardará en el mismo directorio en el que guardaste el archivo `.ipynb` una imagen en formato `.png` con la visualización que corresponde al archivo: 

<img src="https://i.imgur.com/uQnnu1l.png" width="700">

# Otros recursos
- Puedes visualizar los reportes de movilidad de google por estado, desde el código incluido en mi repo [mobility-covid19](https://github.com/jballesterosc/mobility-covid19)
- [Irving Morales](https://https://twitter.com/moaimx) [(@irvingfisica)](https://github.com/irvingfisica) tiene un tutorial de dos partes en Medium para visualizar los mismos datos de la Secretaría de Salud, bastante bien explicado. Puedes encontrar la [parte 1 aquí.](https://medium.com/@irvingmoralesagiss/analizando-datos-de-covid19-en-méxico-pt-1-e177d17b3591)
- Para visualizar mapas a escala nacional o estatal, está la repo [covidmx](https://github.com/FedericoGarza/covidmx) de [Federico Garza](https://twitter.com/fede_gr).

---------

<sup>1</sup> Datos procesados a partir de los oficiales publicados por la [Secretaría de Salud](https://www.gob.mx/salud/documentos/datos-abiertos-152127).
