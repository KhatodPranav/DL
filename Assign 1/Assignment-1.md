# Assignment 1 — TensorFlow / Keras Neural Network

**Aim:** Build a simple neural network in TensorFlow/Keras for handwritten digit classification.

## Concepts
- Artificial Neural Network (ANN)
- Sequential model
- Flatten layer (2D image → 1D vector)
- Dense (fully connected) layers
- ReLU (hidden) and Softmax (output) activations
- Adam optimizer
- Sparse categorical cross-entropy loss
- Training vs test evaluation
- Saving a trained model

## Dataset
- **MNIST** (handwritten digits 0–9)
- 60,000 train images, 10,000 test images
- Each image: 28×28 grayscale
- Preprocessing: pixel values scaled from 0–255 to 0–1

## Tools / Libraries
- TensorFlow / Keras
- Matplotlib (visualize a sample digit)

## Model (high level)
- Flatten (28×28)
- Dense 128 + ReLU
- Dense 10 + Softmax
- Trained for 3 epochs

## Metrics
- Accuracy
- Loss
