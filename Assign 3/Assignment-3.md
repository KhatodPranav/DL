# Assignment 3 — Forward and Backpropagation

**Aim:** Implement forward propagation and backpropagation with TensorFlow/Keras. Study the effect of learning rate and number of epochs.

## Concepts
- Forward propagation
- Backpropagation (weight updates via optimizer)
- Learning rate
- Epochs and batch size
- Validation split
- Underfitting vs overfitting (train vs validation curves)
- Multi-class classification

## Dataset
- **MNIST** handwritten digits
- Images flattened to 784 features
- Normalized by dividing pixels by 255.0

## Tools / Libraries
- TensorFlow / Keras (`Sequential`, `Dense`, `Adam`)
- Pandas (result tables)
- Matplotlib (plots)

## Model (high level)
- Dense 128 + ReLU
- Dense 64 + ReLU
- Dense 10 + Softmax
- Loss: sparse categorical cross-entropy
- Optimizer: Adam (learning rate varied)

## Experiments
- Learning rates: 0.1, 0.01, 0.001 (5 epochs, batch size 128)
- Epochs: 5, 10, 20 (learning rate 0.001, validation split 0.2)
- Full 20-epoch run to plot accuracy and loss

## Metrics
- Test accuracy
- Training / validation accuracy and loss
