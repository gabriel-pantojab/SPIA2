# **Redes Neuronales Recurrentes**

Son un tipo de redes neuronales para procesar datos secuenciales o de series temporales.

La característica principal son sus conexiones recurrentes, este decir la salida de la red en un paso de tiempo se convierte en la entrada para el siguiente paso de tiempo.

## **Neurona Recurrente**

![Alt text](./assets/neuR.png)

En una neurona recurrente la información no solo fluye en una dirección tambien se guarda en la memoria interna que luego es usada para producir una salida en el siguiente paso de tiempo.

La memoria se actualiza con la entrada actual y con el valor de la memoria anterior.

## **¿Cúando utilizar las Redes Nueronales Recurrentes?**

Cuando se tiene una secuencia de datos conocida como secuencias o series temporales, como:
  - Videos
  - Notas Musicales
  - Palabras
  - El clima

## **¿Cómo funcionan las Redes Neuronales Recurrentes?**

![Alt text](./assets/neuR3.png)

Lo que hace una ***RNN*** es que la salida tambien es la retroalimentación de tal manera que se convierte en la entrada del siguiente estado.


## **¿Cómo puede predecir el siguiente carácter en la secuencia? ¿Dónde está la memoria de la Neurona?**

![](./assets/neuR2.png)

En la figura en cada instante de tiempo la neurona tiene dos entradas y dos salidas, las entradas son el dato actual **Xt** y la activación anterior **A(t – 1)** mientras que las salidas son la predicción actual **Yt** y la activación actual **At**, esta activación de salida recibe el nombre de estado oculto, esta es la activación que corresponde precisamente a la memoria de la red, pues permite preservar y compartir la información entre un instante de tiempo y otro.

## **Tipos de Redes Neuronales Recurrentes**

**RNN one-to-one**

![Alt text](./assets/one-to-one.png)

Permite una sola entrada y una única salida. Tiene tamaño de entrada y salida fijos.

Se usa en la clasificación de imagenes.

## **RNN one-to-many**

![](./assets/one-to-many.png)

Toma una sola entrada y produce una secuencia de salidas.

Un ejemplo es el proceso de generación de subtítulos para videos o imágenes.

## **RNN many-to-many**

Many-to-many se utiliza para generar una secuencia de datos de salida a partir de una secuencia de unidades de entrada.

Se divide en dos subcategorias:

- **Equal unit size:** En este caso, el número de unidades tanto de entrada como de salida es el mismo.
  
  ![Alt text](./assets/many-to-many.png)

- **Unequal Unit Size:** las entradas y salidas tienen un número diferente de unidades.
  
  ![](./assets/unequal-unit-size.png)


## **RNN y la retropropagación (backpropagation) a través del tiempo**

**Backpropagation**

La retropropagación se utiliza para calcular el gradiente de una función de error con respecto a los pesos de una red neuronal. El algoritmo trabaja en reversa a través de las distintas capas de gradientes para encontrar la derivada parcial de los errores con respecto a los pesos. Luego, la retropropagación utiliza estos pesos para disminuir los márgenes de error durante el entrenamiento.

Esas derivadas son luego utilizadas por el descenso de gradiente, un algoritmo que puede minimizar iterativamente una función dada. Luego, ajusta los pesos hacia arriba o hacia abajo, dependiendo de cuál disminuya el error.




