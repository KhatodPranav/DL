# Assignment 2 — Multi-Layer Perceptron (MLP)

**Aim:** Use an MLP classifier and compare performance on standard tabular datasets.

## Concepts
- Multi-Layer Perceptron
- Train–test split
- Feature scaling (StandardScaler)
- Hidden layers and ReLU
- Adam solver
- Overfitting / robustness across different splits
- Cross-validation (10-fold)
- Confusion matrix and classification report

## Datasets

**Part A — Iris**
- sklearn Iris dataset (3 flower classes)
- Split: 80% train, 20% test
- MLP: two hidden layers of size 10 each

**Part B — Wine**
- sklearn Wine dataset (3 wine classes)
- Scenario 1: 70% train / 30% test
- Scenario 2: 90% train / 10% test
- MLP1: hidden layers (100, 100)
- MLP2: hidden layer (50)

## Tools / Libraries
- scikit-learn (`MLPClassifier`, datasets, metrics)
- NumPy
- Matplotlib

## Metrics
- Accuracy, Precision, Recall, F1-score
- Confusion matrix
- Loss curve
- 10-fold CV F1 (Wine)
