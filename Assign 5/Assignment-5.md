# Assignment 5 — RNN vs GRU vs LSTM Comparison

**Aim:** Compare SimpleRNN, GRU, and LSTM architectures for binary sentiment classification on the IMDB movie reviews dataset.

## Concepts
- Recurrent Neural Network (SimpleRNN)
- Gated Recurrent Unit (GRU)
- Long Short-Term Memory (LSTM)
- Word embeddings
- Padding / truncating sequences to fixed length
- Binary sentiment classification
- Sigmoid output
- Binary cross-entropy loss
- Early stopping and learning rate reduction callbacks
- Dropout and L2 regularization
- ROC and Precision-Recall curves

## Dataset
- **IMDB** movie reviews (Keras)
- Vocabulary: 10,000 most frequent words
- Sequence length: 200 tokens (padded / truncated)
- 25,000 train reviews, 25,000 test reviews
- Classes: negative (0) and positive (1)
- Balanced class distribution (50% / 50%)

## Tools / Libraries
- TensorFlow / Keras (`Embedding`, `SimpleRNN`, `GRU`, `LSTM`, `Dense`, `Dropout`)
- Keras callbacks (`EarlyStopping`, `ReduceLROnPlateau`)
- scikit-learn (accuracy, precision, recall, F1, ROC-AUC, confusion matrix, classification report)
- NumPy, Pandas (result tables)
- Matplotlib, Seaborn (plots and heatmaps)

## Models (high level)

**SimpleRNN**
- Embedding (10,000 → 64-dim)
- SimpleRNN 64 units + Dropout
- Dense 1 + Sigmoid

**GRU**
- Embedding (10,000 → 64-dim)
- GRU 64 units + Dropout
- Dense 1 + Sigmoid

**LSTM**
- Embedding (10,000 → 64-dim)
- LSTM 64 units + Dropout
- Dense 1 + Sigmoid

- All models: Adam optimizer, binary cross-entropy loss
- Trained with early stopping and learning rate scheduling

## Metrics
- Accuracy, Precision, Recall, F1-score
- ROC-AUC score
- Confusion matrix
- Training vs validation accuracy and loss curves
- ROC and Precision-Recall curves
- Comparative summary table across all three architectures