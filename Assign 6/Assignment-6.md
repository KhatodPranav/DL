# Assignment 6 — CNN for Image Classification

**Aim:** Design a Convolutional Neural Network for plant-leaf disease image classification (Tomato / Soybean type disease dataset).

## Concepts
- Convolutional Neural Network (CNN)
- Convolution filters (edges, texture, spots)
- Max pooling
- Flatten + Dense layers
- Dropout (reduce overfitting)
- Image resizing and pixel rescaling (0–255 → 0–1)
- Train / validation split
- Softmax multi-class output

## Dataset
- Plant leaf disease images (folder-wise classes: healthy / diseased)
- Images resized (e.g. 128×128)
- Split: 80% training, 20% validation
- Batch size: 32

## Tools / Libraries
- TensorFlow / Keras (`Conv2D`, `MaxPooling2D`, `Dense`, `Dropout`)
- kagglehub (dataset download)
- Matplotlib, NumPy
- scikit-learn (confusion matrix, classification report)
- seaborn (heatmap)

## Model (high level)
- Rescaling layer
- Conv 32 → MaxPool
- Conv 64 → MaxPool
- Conv 128 → MaxPool
- Flatten → Dense 128 + ReLU → Dropout 0.5
- Softmax output (number of disease classes)
- Optimizer: Adam (lr 0.0001)
- Loss: sparse categorical cross-entropy
- Epochs: 10

## Metrics
- Accuracy
- Precision, Recall, F1-score
- Confusion matrix
- Training vs validation accuracy and loss plots
