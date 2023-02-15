### Introducción

En este repositorio encontrará el código fuente de los modelos implementados para la fase experimental del trabajo "Sistema inteligente de recomendación de moda basado en Deep Learning". 

### Contenido
#### 1. Encoder ConvLSTM with Data Augmentation
En este experimento se utiliza un codificador espacio temporal (ConvLSTM) de 4 capas y luego se utiliza un clasificador de 3 capas densas. Adicionalmente, se implementa la técnica de "data augmentation", para mejorar la predicción del modelo. Este es el modelo principal de nuestro estudio. 

#### 2. Encoder ConvLSTM without Data Augmentation
Este escensario es bastante similar al primero, ya que se utiliza la misma arquitectura del modelo, pero sin utilizar "data augmentation", de manera que si se generan cambios en la precisión del modelo.

#### 3. Encoder CNN
Para el tercer modelo no se utilizó el codificador espacio temporal, sino dos capas convolucionales normales con sus respectivas capas de “max pooling”. En este escenario se utilizó igualmente un clasificador de 3 capas densas.

#### 4. Autoencoder ConvLSTM
En este escensario se utilizó un autocodificador completo. A diferencia de los tres escenarios anteriores, aquí se utiliza tanto 4 capas convolucionales recurrentes para el codificador y 4 capas convolucionales recurrentes para el decodificador, además de las capas densas de clasificación. 

#### 5. Autoencoder CNN
Aquí se emplean 2 capas convolucionales para el codificador y 2 capas convolucionales para el decodificador. Luego de cada capa convolucional en el codificador, se tiene una capa de “max pooling”, mientras que para el decodificador, se tiene una capa de “UpSampling” luego de cada capa convolucional. 
