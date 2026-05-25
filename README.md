# Game Player Segmentation with K-Means

## Descripción del proyecto

Este proyecto aplica técnicas de aprendizaje no supervisado para segmentar jugadores de videojuegos en función de su comportamiento dentro del juego.

El análisis se basa en dos variables principales:

- `daily_hours_spent`: media diaria de horas que el jugador pasa jugando.
- `daily_currency_spent`: media diaria de dinero virtual que el jugador gasta dentro del juego.

A partir de estas variables, se utiliza el algoritmo K-Means para identificar grupos de jugadores con comportamientos similares. El objetivo es descubrir patrones dentro de los datos y traducirlos en información útil para la toma de decisiones de negocio.

Este proyecto forma parte de un ejercicio práctico de clustering, desarrollado en Python mediante un notebook, utilizando principalmente la librería Scikit-learn.

---

## Objetivo

El objetivo principal del proyecto es realizar una segmentación de jugadores mediante K-Means, identificando perfiles diferenciados según el tiempo de juego y el gasto en moneda virtual.

Este tipo de análisis puede ayudar a una empresa de videojuegos a comprender mejor a sus usuarios y diseñar estrategias más personalizadas.

Los objetivos específicos del proyecto son:

- Cargar y explorar el dataset.
- Visualizar la relación entre las variables principales.
- Aplicar el método del codo para seleccionar el número adecuado de clústeres.
- Entrenar un modelo K-Means.
- Visualizar los clústeres obtenidos.
- Representar los centroides de cada clúster.
- Evaluar la calidad del clustering mediante métricas internas.
- Interpretar los resultados desde una perspectiva de negocio.

---

## Dataset

El dataset utilizado se denomina `game_players.csv`.

Cada fila representa un jugador.

Las variables incluidas son:

| Variable | Descripción |
|---|---|
| `daily_hours_spent` | Media diaria de horas que el jugador pasa jugando |
| `daily_currency_spent` | Media diaria de dinero virtual que el jugador gasta dentro del juego |

El dataset permite analizar la relación entre el nivel de actividad del jugador y su gasto dentro del videojuego.

---

## Metodología

El proyecto sigue una estructura práctica de análisis no supervisado:

1. Carga del dataset.
2. Revisión inicial de los datos.
3. Visualización de las variables principales.
4. Análisis visual para identificar posibles agrupaciones.
5. Aplicación del método del codo.
6. Selección del número óptimo de clústeres.
7. Entrenamiento del modelo K-Means.
8. Asignación de cada jugador a un clúster.
9. Visualización final de los clústeres y centroides.
10. Evaluación del clustering mediante métricas internas.
11. Interpretación de los resultados desde una perspectiva de negocio.

---

## Fundamento técnico

K-Means es un algoritmo de aprendizaje no supervisado utilizado para agrupar observaciones en función de su similitud.

El algoritmo parte de un número definido de clústeres, representado por el parámetro `k`. A continuación, asigna cada observación al centroide más cercano y recalcula los centroides de forma iterativa hasta estabilizar la agrupación.

En este proyecto, cada jugador se representa mediante dos variables: horas diarias de juego y gasto diario en moneda virtual. A partir de esta información, K-Means permite identificar segmentos de jugadores con patrones similares.

---

## Elbow Method

Para seleccionar el número adecuado de clústeres se utiliza el Elbow Method.

Este método consiste en entrenar varios modelos K-Means con diferentes valores de `k` y observar cómo disminuye la inercia.

La inercia mide la suma de las distancias de los puntos respecto al centroide de su clúster. A medida que aumenta el número de clústeres, la inercia disminuye. Sin embargo, llega un punto en el que añadir más clústeres apenas mejora el resultado.

Ese punto de cambio se interpreta como el posible número óptimo de clústeres.

---

## Librerías utilizadas

El proyecto se ha desarrollado en Python utilizando las siguientes librerías:

- pandas
- numpy
- matplotlib
- seaborn
- plotly
- scikit-learn

---



## Resultados principales

El análisis permite identificar tres perfiles principales de jugadores:

1. Jugadores con bajo tiempo de juego y bajo gasto en moneda virtual.
2. Jugadores con mayor tiempo de juego y gasto moderado.
3. Jugadores con alto tiempo de juego y alto gasto en moneda virtual.

Esta segmentación permite comprender mejor los distintos comportamientos de los usuarios dentro del videojuego.

---

## Valor de negocio

La segmentación de jugadores puede aportar valor a una empresa de videojuegos porque permite transformar datos de comportamiento en perfiles accionables.

A partir de los clústeres obtenidos, la empresa podría diseñar estrategias diferenciadas para cada grupo de jugadores.

Por ejemplo:

- Para jugadores con alto gasto, se podrían ofrecer recompensas premium, contenido exclusivo o programas de fidelización.
- Para jugadores activos con gasto moderado, se podrían crear promociones personalizadas para incentivar compras dentro del juego.
- Para jugadores con baja actividad, se podrían diseñar campañas de reactivación.
- Para jugadores con alto tiempo de juego, se podrían analizar oportunidades de retención y mejora de la experiencia.

Este tipo de análisis ayuda a pasar de una visión general de los usuarios a una comprensión más segmentada y útil para la toma de decisiones.

---

## Métricas de evaluación

Aunque el clustering no utiliza una variable objetivo, se pueden emplear métricas internas para evaluar la calidad de los grupos obtenidos.

En el proyecto se consideran métricas como:

- Inercia.
- Silhouette Score.
- Davies-Bouldin Index.

Estas métricas ayudan a valorar la separación entre clústeres y la coherencia interna de los grupos.

---

## Conclusión

Este proyecto demuestra cómo aplicar aprendizaje no supervisado para segmentar jugadores de videojuegos mediante K-Means.

A partir de dos variables sencillas, el modelo permite identificar patrones diferenciados de comportamiento y traducirlos en información útil para negocio.

El ejercicio combina análisis exploratorio, visualización, modelado no supervisado, evaluación e interpretación de resultados, mostrando una aplicación práctica de Machine Learning en un contexto de videojuegos.

---

## Autora

Paola Albán  
Data Analytics | Business Intelligence | Machine Learning aplicado

GitHub: [PaoAlbanData](https://github.com/PaoAlbanData)
