# clasificador-cancer-mama
Clasificador de un cáncer de mama basado en 30 medidas numéricas, se entrenó en 3 modelos y al final se concluye cuál es el mejor.

El ejercicio planteado es el siguiente:

Basándose en el dataset de Breast Cancer Wisconsin Diagnostic que tiene características de muestras de mujeres que tienen cáncer de mama, se propone entrenar 3 modelos de Machine Learning, evaluarlos con un conjunto de datos de test y determinar cuál es el mejor, considerando que un falso positivo no es tan preocupante como un falso negativo, ya que en el futuro se le hacen más pruebas a las pacientes y hay oportunidades de descubrir que estábamos en un error.

Sin embargo, un falso negativo puede llevar a que el cáncer se desarrolle sin supervisión durante más tiempo del necesario y podría llevar a daños más graves o incluso la muerte de la paciente.

Los modelos seleccionados fueron: RandomForest, GradientBoosting y Red Neuronal Dense.

Escogí esos modelos por buenas experiencias anteriores obtenidas, por sus características optimizadas con respecto a otros modelos, y porque son de los más recientes.

Para este trabajo se realizó una separación del dataset en 20% para Test y 80% para entrenamiento.

Después de entrenar y de evaluar los 3 modelos se obutvieron los siguientes accuracy:
RandomForest -> 100%
GradientBoosting -> 96%
Red Neuronal Dense -> 92%

Sin dudar y con la ayuda de las matrices de confusión el mejor modelo en predecir fue el RandomForest, y como se sugirió también, los falsos negativos fueron "0", que ese parámetro era el más preocupante.
También hay que considerar que para el RandomForest sólo fue necesario un "n_estimators" de 10, lo cuál aún optimiza recursos y tiempo. 
