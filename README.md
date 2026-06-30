# MNIST Digit Classification using Neural Networks

A beginner-friendly deep learning project that builds and trains a simple feedforward Artificial Neural Network (ANN) using TensorFlow/Keras to classify handwritten digits (0–9) from the classic MNIST dataset.

## Project Overview

The goal of this project is to demonstrate the end-to-end workflow of an image classification task using neural networks — from loading and visualizing data, through model building and training, to evaluation and inference on individual images.

## Dataset

- **Source:** MNIST handwritten digits dataset (standard `60,000` training / `10,000` test split)
- **Image size:** 28x28 grayscale pixels
- **Classes:** 10 (digits 0–9)
- **File:** `dataset/mnist.npz` (contains `x_train`, `y_train`, `x_test`, `y_test` arrays)

## Project Structure

```
mnist_digit_classification/
│
├── asset/
│   └── 3-digit.PNG                    # Test Image
│
├── output/
│   └── confusion-matrix.PNG        # saved confusion matrix
│
├── MNIST-Digit-Classification.ipynb # Main Jupyter notebook
└── README.md
```

## Model Architecture

A simple fully connected (feedforward) neural network:

| Layer            | Type    | Output Shape | Activation |
|-------------------|---------|--------------|------------|
| Flatten           | Input   | (784,)       | —          |
| Hidden Layer      | Dense   | (128,)       | ReLU       |
| Output Layer      | Dense   | (10,)        | Softmax    |

- **Epochs:** 10
- **Batch Size:** 32


## Workflow Steps

1. Import required libraries (NumPy, Matplotlib, TensorFlow/Keras)
2. Load the MNIST dataset
3. Inspect dataset shapes and label ranges
4. Visualize sample digit images
5. Normalize pixel values to the [0, 1] range
6. Build the neural network
7. Compile the model
8. Train the model for 10 epochs with validation
9. Evaluate test accuracy and visualize a confusion matrix
10. Generate predictions on the test dataset
11. Predict a single image's digit
12. Display the predicted digit alongside the actual test image

## How to Run

1. Install dependencies
2. Open `MNIST_Digit_Classification.ipynb` in Jupyter Notebook or Google Colab.
3. Run all cells sequentially from top to bottom.

## Tech Stack

- Python 3.x    #Tensorflow doesn't support python 3.14 yet, so ensure that you are using python 3.11.x to 3.13.x
- TensorFlow / Keras
- NumPy
- Matplotlib

