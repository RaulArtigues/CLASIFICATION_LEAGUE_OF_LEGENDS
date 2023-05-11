# CLASIFICATION_LEAGUE_OF_LEGENDS

Este conjunto de datos contiene los primeros 10 minutos. estadísticas de aprox. 10k juegos clasificados (SOLO QUEUE) de un ELO alto (DIAMOND I a MASTER). Los jugadores tienen aproximadamente el mismo nivel.
Cada juego es único. El gameId puede ayudarlo a obtener más atributos de la API de Riot.
Hay 19 funciones por equipo (38 en total) recopiladas después de 10 minutos en el juego. Esto incluye asesinatos, muertes, oro, experiencia, nivel... Depende de usted hacer un poco de ingeniería de funciones para obtener más información.
La columna blueWins es el valor objetivo (el valor que intentamos predecir). Un valor de 1 significa que el equipo azul ha ganado. 0 de lo contrario.

Objetivos del presente proyecto
Efectuar una red neuronal sobre un dataset propio a poder ser siguiendo cualquiera de los tutoriales de la documentación de Tensorflow. El objetivo del ejercicio es poner en práctica el concepto de "prototipado rápido" y cruzar la línea para empezar a trabajar en un problema real.
Se requiere probar 2 arquitecturas. Es decir, 2 funciones de creación de modelo dinámicas como las vistas en clase que serán las usadas en el grid search de hiper parámetros. 
Se requiere una búsqueda de hiperparámetros. 
Una vez elegido un modelo, hacer un grid search cambiando únicamente uno de los hyper parámetros. Estudiar cuál es su efecto y comprobar que sea el esperado a corde a los notebooks vistos en clase "nn_architecture". Se requiere estudiar 3 parámetros (learning rate, batch size, drop_out, activaciones, escalado de variables, etc. a elegir 3) Hacer un cambio sobre las las variables (feature engineering) y ver cúal es el efecto sobre el modelo. 

Guia
A continuación se describen los pasos y la estrucutura del presente proyecto: 
1- Eliminación de valores atípicos y estandarización de los datos. 
2- Creación del Modelo lineal para saber el feedback y si con una red neuronal predice la victoria del equipo Rojo y Azul. 
3- Creación de una red neuronal con varias capas densas en forma de limon, es decir, el número de neuronas ira aumentado hasta llegar al "climactic moment" y a partir de este momento las neuronas en cada capa densa irán disminuyendo. 
4- Creación de una red neuronal con varias capas densas en forma decreciente, es decir, el número de neuronas ira disminuyendo hasta llegar al "climactic moment" que se cree oportuno. 
5- Con las 3 arquitecturas creadas realizar grid search inicial. 
6- Elección del modelo, tipo de forma de la arquitectura de la Red Neuronal. 
7- Cambiar 3 hiper parámetros y comparar los resultados con la red anterior: Regularización; Activación y Función de Pérdida; Batch Size y Dense Layers. 
8- Realizar una selección de variables y aplicar la red neuronal óptima anterior y comparar los resultados. 
9- Conclusión y elección de la red neuronal óptima.
