# Image classification with neural networks

This project demonstrates **automatic image classification** for an e-commerce store using a **neural network** implemented in **tensorFlow** and **keras**. The model is trained on the **fashion MNIST dataset**, which contains grayscale images of clothing items.

## Features

- **Data loading and exploration**
  - Loads the Fashion MNIST dataset directly from Keras.
  - Explores dataset shape, label ranges, and sample images.
  - Visualizes sample images with their respective labels.

- **Data preprocessing**
  - Normalizes image pixel values to the range `[0, 1]`.
  - Labels are mapped to human-readable class names (e.g., T-shirt, Pants, Dress).

- **Model creation, compilation, and training**
  - Uses a simple neural network with layers: Flatten → Dense (ReLU) → Dropout → Dense (Softmax).
  - Compiles the model with `adam` optimizer and `sparse_categorical_crossentropy` loss.
  - Trains the model for 5 epochs with validation split.

- **Model saving and loading**
  - Saves the trained model to a file using `model.save()`.
  - Loads the saved model using `load_model()` for later inference.

- **Model evaluation**
  - Visualizes training and validation accuracy and loss per epoch.
  - Tests the model on the test set and compares predictions with actual labels.

- **Neural network visualization**
  - Graphical representation of the model's structure and nodes.
  - Displays connections between Flatten, ReLU, and Softmax layers.

## Installation

The project requires **Python 3** and the following libraries:

```python
import numpy as np
import matplotlib.pyplot as plt
import tensorflow as tf
from tensorflow import keras
from keras.models import load_model
```

## Usage

- Load the Fashion MNIST dataset.  
- Preprocess images and labels.  
- Create, compile, and train the neural network.  
- Save and reload the trained model.  
- Visualize accuracy and loss over epochs.  
- Test the model and visualize predictions.  
- Optional: visualize the neural network structure.  

## Notes

- This project is designed as a prototype for learning and experimentation.  
- Training and evaluation can be done on a standard CPU, but a GPU will speed up the process.  
- The model is simple and intended for educational purposes; real e-commerce applications may require more complex architectures.  

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute the code as needed.
