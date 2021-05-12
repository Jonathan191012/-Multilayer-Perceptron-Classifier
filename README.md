# Multilayer perceptron classifier
## ¿Qué son los perceptrones multicapa?


El perceptrón es muy útil para clasificar conjuntos de datos que son linealmente separables. Se encuentran con serias limitaciones con conjuntos de datos que no se ajustan a este patrón como se descubrió con el problema XOR. El problema XOR muestra que para cualquier clasificación de cuatro puntos existe un conjunto que no es separable linealmente.

MultiLayer Perceptron (MLP) rompe esta restricción y clasifica conjuntos de datos que no son separables linealmente. Lo hacen utilizando una arquitectura más robusta y compleja para aprender modelos de regresión y clasificación para conjuntos de datos difíciles.

## ¿Cómo funciona?

El perceptrón multicapa esta compuesto por una capa de entrada, una capa de salida y n capas ocultas entremedias.
Se caracteriza por tener salidas disjuntas pero relacionadas entre sí, de tal manera que la salida de una neurona es la entrada de la siguiente.


En el perceptrón multicapa se pueden diferenciar una 2 fases:

- **Propagación** en la que se calcula el resultado de salida de la red desde los valores de entrada hacia delante.
  
- **Aprendizaje** en la que los errores obtenidos a la salida del perceptrón se van propagando hacia atrás (backpropagation) con el objetivo de modificar los pesos de las conexiones para que el valor estimado de la red se asemeje cada vez más al real, este aproximación se realiza mediante la función gradriente del error.

## Arquitectura

Las capas pueden clasificarse en tres tipos:

- **Capa de entrada**: Constituida por aquellas neuronas que introducen los patrones de entrada en la red. En estas neuronas no se produce procesamiento.  Las neuronas de la capa de entrada no actuan como neuronas propiamente dichas, sino que se encargan unicamente de recibir las señales o patrones del exterior y propagar dichas señales a todas las neuronas de la siguiente capa
  
- **Capas ocultas**: Formada por aquellas neuronas cuyas entradas provienen de capas anteriores y cuyas salidas pasan a neuronas de capas posteriores. Las neuronas de las capas ocultas realizan un procesamiento no lineal de los patrones recibidos.

  
- **Capa de salida**: Neuronas cuyos valores de salida se corresponden con las salidas de toda la red.  La ultima capa actua como salida de la red, proporcionando al exterior la respuesta de la red para cada uno de los patrones de entrada.

