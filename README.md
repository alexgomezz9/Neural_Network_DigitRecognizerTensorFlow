# Reconocimiento de Dígitos con Redes Neuronales

Este proyecto utiliza redes neuronales para resolver el problema de **reconocimiento de dígitos escritos a mano** (del 0 al 9) usando el famoso conjunto de datos **MNIST**. El objetivo principal es entrenar un modelo que pueda identificar correctamente los dígitos en imágenes de 28x28 píxeles.

## Descripción del Proyecto

- Se utiliza **TensorFlow** y **Keras** para construir y entrenar una red neuronal profunda que clasifica las imágenes de dígitos.
- El modelo es entrenado con el conjunto de datos **MNIST**, que contiene miles de imágenes de dígitos escritos a mano con sus correspondientes etiquetas.
- Una vez entrenado el modelo, este genera predicciones para un conjunto de prueba sin etiquetas.
- El resultado final se guarda en un archivo `submission.csv`, que contiene las predicciones de la red neuronal para cada imagen de prueba.

## Funcionamiento del Modelo

- El modelo está compuesto por una red neuronal con capas densas (fully connected) y utiliza **ReLU** como función de activación en las capas ocultas, y **softmax** en la capa de salida para la clasificación en 10 clases (dígitos del 0 al 9).
- Se entrena utilizando el optimizador **Adam** y la función de pérdida **sparse categorical crossentropy**.
- Se monitorea la precisión y la pérdida tanto en el conjunto de entrenamiento como en el de validación para evitar el sobreajuste y garantizar un buen rendimiento.

## Resultados

El modelo alcanza una precisión en el conjunto de validación de aproximadamente **96-97%** después de algunas épocas de entrenamiento, lo que indica que es capaz de generalizar bien y realizar predicciones precisas sobre los dígitos escritos a mano.
