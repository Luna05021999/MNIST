## 🧠 Clasificación de Dígitos con Red Neuronal Convolucional en MNIST 🖌️

Este proyecto implementa una Red Neuronal Convolucional (CNN) usando TensorFlow y Keras para clasificar dígitos escritos a mano del dataset MNIST. La aplicación final permite a los usuarios dibujar un dígito y ver la predicción del modelo en tiempo real a través de una interfaz interactiva creada con Gradio.

## 📜 Descripción

La red neuronal está entrenada para clasificar dígitos del 0 al 9 usando el conocido conjunto de datos MNIST, que contiene imágenes de dígitos en escala de grises de 28x28 píxeles. El proyecto incluye:

Preprocesamiento de datos 📊
Construcción de una red neuronal convolucional (CNN) en Keras 🧠
Entrenamiento y evaluación del modelo 📈
Visualización de la arquitectura del modelo usando Netron 👀
Interfaz gráfica de usuario (GUI) para probar el modelo en tiempo real con Gradio 🖌️

## 📂 Contenido del Proyecto

- 🧠 Entrenamiento del modelo CNN: Código para construir, entrenar y evaluar la CNN en Keras.
- 👀 Visualización del modelo con Netron: Herramienta para ver la estructura del modelo.
- 🌐 Interfaz con Gradio: Aplicación web simple para probar el modelo en tiempo real.

## 🛠️ Requisitos

Este proyecto requiere Python 3 y las siguientes librerías de Python:

tensorflow (para construir y entrenar el modelo CNN)
numpy (para manipulación de datos)
matplotlib (para visualización de datos)
gradio (para crear la interfaz de usuario interactiva)
netron (para visualizar la arquitectura del modelo)

## 🚀 Instrucciones de Uso

Clona el repositorio o descarga los archivos de este proyecto.

Entrena el modelo (opcional, si deseas reentrenarlo):

Si deseas reentrenar el modelo, abre el notebook y ejecuta las celdas correspondientes. El modelo se entrenará usando el conjunto de datos MNIST, y se guardará como mnist_model.keras.

Ejecuta la Interfaz de Usuario con Gradio:

Después de cargar o entrenar el modelo, puedes ejecutar la interfaz interactiva de Gradio para probar el modelo en tiempo real.

🔍 Explicación del Código
Carga de Datos: Se usa el conjunto de datos MNIST proporcionado por tensorflow.keras.datasets, que se divide en conjuntos de entrenamiento y prueba.

Preprocesamiento:

Redimensiona las imágenes a (28, 28, 1) y normaliza los valores de los píxeles a un rango entre 0 y 1.
Construcción del Modelo:

Se define una CNN con capas Conv2D, MaxPooling2D, Flatten, y capas densas para clasificar las imágenes en 10 clases (dígitos del 0 al 9).
Compilación y Entrenamiento:

El modelo se compila con el optimizador Adam y la función de pérdida categorical_crossentropy.
Durante el entrenamiento, se usa un callback de EarlyStopping para detener el entrenamiento si la precisión no mejora después de 2 épocas consecutivas, evitando el sobreajuste.
Evaluación del Modelo:

Se evalúa el modelo en el conjunto de prueba, logrando una precisión cercana al 99%.
Guardado del Modelo:

El modelo entrenado se guarda en mnist_model.keras para su reutilización.
Interfaz de Usuario con Gradio:

La interfaz permite que los usuarios dibujen un dígito y obtengan la predicción del modelo.

## 🎨 Ejemplo de Uso

Una vez que ejecutes la interfaz de Gradio, verás un lienzo donde puedes dibujar un dígito (0-9).
Haz clic en Submit y el modelo mostrará el dígito predicho.

## 📊 Resultados

El modelo logra una precisión de aproximadamente 99% en el conjunto de prueba, lo que demuestra su eficacia en la clasificación de dígitos escritos a mano.

## 📝 Conclusiones

Este proyecto demuestra cómo implementar una red neuronal convolucional para resolver un problema de clasificación de imágenes usando TensorFlow y Keras. La integración con Gradio permite probar el modelo de manera interactiva, y Netron facilita la inspección de la arquitectura del modelo. Este enfoque es ideal para tareas de clasificación de imágenes y demuestra la potencia de las CNNs en problemas de visión por computadora.

## Contacto
Luna Outerelo Fernández.
Email: lunaouterelo9@gmail.com
Linkedin: https://www.linkedin.com/in/luna-outerelo-4414a0192/
