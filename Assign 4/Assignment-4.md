# Assignment 4 — Simple RNN for Sequence Classification

**Aim:** Classify IMDB movie reviews as positive or negative using a Simple RNN.

## Concepts
- Recurrent Neural Network (SimpleRNN)
- Sequential / text data
- Word embeddings
- Padding / truncating sequences to fixed length
- Binary sentiment classification
- Sigmoid output
- Binary cross-entropy loss

## Dataset
- **IMDB** movie reviews (Keras)
- Vocabulary: 10,000 most frequent words
- Sequence length: 200 tokens (padded)
- 25,000 train reviews, 25,000 test reviews
- Classes: negative (0) and positive (1)

## Tools / Libraries
- TensorFlow / Keras (`Embedding`, `SimpleRNN`, `Dense`, `pad_sequences`)
- NumPy, Matplotlib
- scikit-learn metrics

## Model (high level)
- Embedding (10,000 words → 64-dim vectors)
- SimpleRNN with 64 units
- Dense 1 + Sigmoid
- Optimizer: Adam
- 3 epochs, batch size 128, validation split 0.2

## Metrics
- Accuracy, Precision, Recall, F1-score
- Confusion matrix
- Train vs validation accuracy curve
