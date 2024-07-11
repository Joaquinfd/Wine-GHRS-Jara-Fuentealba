# Wine-GHRS-Jara-Fuentealba

| Nombre             | Email               |
|--------------------|---------------------|
| Joaquín Fuentalba  | jffuentealba@uc.cl  |
| Martín Jara        | martinjf@uc.cl      |

Abstract
Las ventas de vino se han reducido considerablemente debido a la
poca información sobre cual variedad es más ad hoc a los consum-
idores. En base a esto, se busca utilizar un modelo híbrido donde
se extrae información de los usuarios que han calificados otros
vinos mezclado con un grafo de similitud entre usuarios, para así
entregar una recomendación cercana a lo que desea el consumi-
dor. Este artículo se basa en el método desarrollado por los autores
Darban y Valipour [ 9 ] donde realizan la experimentación con el
conocido dataset MovieLens. Los resultados de nuestro experimento
nos demuestran que el método sigue siendo efectivo con métricas
similares, aún cambiando el dominio de recomendación.

## Librerías Requeridas

Este proyecto requiere las siguientes librerías de Python:

- `numpy`
- `pandas`
- `scipy`
- `networkx`
- `itertools`
- `collections`
- `sklearn.preprocessing`
- `pickle`
- `matplotlib`
- `seaborn`
- `torch`
- `torch.nn`
- `torch.optim`
- `sklearn`

Para instalar las dependencias necesarias:

```bash
pip install numpy pandas scipy networkx matplotlib seaborn torch scikit-learn
```

Este proyecto consta de 2 archivos principales y necesarios para el funcionamiento, `wines-graph.ipynb` y `wines-recommender.ipynb`. Solbre la metodología se puede tener una versión completa leyendo nuestro paper. El archivo `wines-gaph.ipynb` cumple la función de elaborar el grafo de usuarios y combinar los datos demográficos de usuario con los datos del grafo. Todo los archivos que lee el código estan disponibles en este repositorio, al igual que todos los directorios en los que se guardan archivos como funcionamiento del código.


```bash
├── data_wines
│   ├── encoded_features
│       ├── encoded_features.pkl
│   ├── graph_alpha_0.01.pkl
│   ├── graph_alpha_0.002.pkl
│   ├── graph_alpha_0.005.pkl
│   └──  x_train_alpha(0.002).pkl
├── models
│   └── autoencoder.pt
├── Datos
│   ├── XWines_Slim_1K_wines.csv
│   ├── XWines_Slim_150K_ratings.csv
│   ├── XWines_Slim_10K_users.csv
│   ├── XWines_Test_1K_ratings.csv
│   └── XWines_Test_100_wines.csv 
├── wines-graph.ipynb
├── wines-recommender.ipynb
├── unpickle.ipynb
└── README.md
```


La ejecución del proyecto consiste de (en el siguiente orden): 
 
- Ejecutar todas las celdas del archivo `wines-graph.ipynb`
- Ejecutar todas las celdas del archivo `wines-recommender.ipynb`

Para visualizar las métricas del grafo, se debe ejecutar el archivo `unpickle.ipynb`


