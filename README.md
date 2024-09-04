# Clasificador de grietas en hormigón

Proyecto final desarrollado para **Certificado profesional de Ingenieria de IA de IBM** a traves de la plataforma coursera.

El proyecto busca generar un modelo capaz de predecir si una determinada imagen correspondiente a una estructura de hormigon contiene o no grietas. A partir del uso de tecnicas de aprendizaje profundo mediante Python y diversas librerias como Keras y TensorFlow, se busca obtener a partir de modelos preentrenados un modelo que permita resolver la problematica planteada de la mejor y mas eficiente manera posible.

Se crearon dos modelos para la clasificacion de grietas, los cuales permitian predecir dos posibles estados (con o sin grietas), a partir de los modelos preentrenados *ResNet-50* y *VGG16*.
ResNet-50 es una arquitectura CNN que pertenece a la familia ResNet (Redes Residuales), una serie de modelos diseñados para abordar los desafíos asociados con el entrenamiento de redes neuronales profundas, mientras que VGG16 es un tipo de CNN (red neuronal convolucional) que se considera uno de los mejores modelos de visión artificial hasta la fecha.
El modelo ResNet-50 cuenta con una profundidad de 50 capas de peso, mientras que para el VGG16 se utilizan 16 de dichas capas.
Para el uso de dichos modelos aplicado al problema que se pretende solucionar en este caso, se reemplaza la  capa superior del modelo pre-entrenado, ya que lo que se busca es definir una capa de salida propia y entrenarla para que este optimizada con el conjunto de datos de imagenes descargado para cada caso.
Una vez entrenados ambos modelos y realizada las respectivas evaluaciones entre los mismos, se optó por el uso del modelo generado a partir del ResNet-50, ya que demostró un mejor rendimiento en comparativa con el modelo generado a partir de VGG16.

El modelo puede ser utilizado desde el siguiente link: *[Clasificador_hormigon](https://colab.research.google.com/github/rodriquiel/concrete_images_classifier/blob/main/Clasificador_imagenes_hormigon.ipynb)*, o tambien desde este mismo repositorio accediendo al colab nombrado **Clasificador_imagenes_hormigon.ipynb**, y siguiendo las detalladas instrucciones con las cuales cuenta el mismo.

Librerias de Python utilizadas:
*  Numpy
*  Matplotlib
*  Keras 
*  TensorFlow
*  PIL

Las imagenes para los entrenamientos, validaciones y pruebas de los modelos fueron otorgadas por IBM SkillsNetwork
