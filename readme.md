# Deep Learning Assignments — Folder Overview

Subject: **Deep Learning**  

---

## Assign 1

**What it is:** First neural network using TensorFlow/Keras.

**Files**
- `Tensorflow&Keras.ipynb` — implementation notebook
- `Assignment-1.md` — short concept note
- `Assignment-1.pdf` — practical write-up

**Dataset:** MNIST (handwritten digits 0–9), 28×28 grayscale, 60k train / 10k test. Pixels scaled 0–1.

**Used:** TensorFlow/Keras Sequential model, Flatten, Dense (128 ReLU + 10 Softmax), Adam, sparse categorical cross-entropy, Matplotlib, 3 epochs.

**Task:** Classify digits and report test accuracy (~97.6%).

---

## Assign 2

**What it is:** Multi-Layer Perceptron (MLP) on two sklearn datasets.

**Files**
- `mlp-classification-on-iris-dataset.ipynb`
- `mlp-classifier-on-wine-dataset.ipynb`
- `Assignment-2.md`
- `Assignment-2.pdf`

**Datasets**
- **Iris** — 3 flower classes, 80/20 split, StandardScaler
- **Wine** — 3 wine classes; Scenario 1 (70/30) and Scenario 2 (90/10)

**Used:** scikit-learn `MLPClassifier`, NumPy, Matplotlib, accuracy / precision / recall / F1, confusion matrix, loss curve, 10-fold CV (Wine).

**Models:** Iris MLP (10, 10); Wine MLP1 (100, 100) vs MLP2 (50).

---

## Assign 3

**What it is:** Forward propagation and backpropagation; effect of learning rate and epochs.

**Files**
- `Forward_Backpropagation_TensorFlow_Keras_Colab.ipynb`
- `Assignment-3.md`
- `Assignment-3.pdf`

**Dataset:** MNIST, flattened to 784 features, normalized /255.

**Used:** Keras Sequential, Dense 128 → 64 → 10 Softmax, Adam, sparse categorical cross-entropy, Pandas, Matplotlib.

**Experiments:** Learning rates 0.1 / 0.01 / 0.001; epochs 5 / 10 / 20; train–val accuracy and loss plots.

---

## Assign 4

**What it is:** Simple RNN for sequence (text) classification.

**Files**
- `Simple_RNN_Sequence_Classification.ipynb`
- `Assignment-4.md`
- `Assignment-4.pdf`

**Dataset:** IMDB movie reviews, 10,000-word vocab, sequences padded to length 200, 25k train / 25k test, binary sentiment.

**Used:** Keras Embedding + SimpleRNN(64) + Dense Sigmoid, Adam, binary cross-entropy, NumPy, Matplotlib, sklearn metrics.

**Task:** Predict positive/negative review; report accuracy, precision, recall, F1, confusion matrix.

---

## Assign 6

**What it is:** CNN for plant-leaf disease image classification.

**Files**
- `cnn-for-image-classification.ipynb`
- `Assignment-6.md`
- `Assignment-6.pdf`

**Dataset:** Leaf disease images from Kaggle (tomato / similar plant-disease set; classes in folders). Images resized (e.g. 128×128), 80/20 train–val, batch size 32.

**Used:** Conv2D + MaxPooling, Flatten, Dense, Dropout 0.5, Softmax, Adam (lr 0.0001), sparse categorical cross-entropy, kagglehub, Matplotlib, sklearn + seaborn for confusion matrix / report.

**Task:** Classify leaf images; plot accuracy/loss and confusion matrix.

---

## Assign 7

**What it is:** Compare four CNN architectures on the same dataset.

**Files**
- `comparing-alexnet-vgg16-resnet50-efficientnet.ipynb`
- `Assignment-7.md`
- `Assignment-7.pdf`

**Dataset:** Pistachio Image Dataset (Kaggle) — 2 classes (`Kirmizi_Pistachio`, `Siirt_Pistachio`), 2148 images, 224×224, ImageNet mean/std normalization, batch 16.

**Used:** TensorFlow/Keras Applications, kagglehub, Pandas, Matplotlib.

**Models (10 epochs, Adam lr 0.001)**
| Model | Approach |
|---|---|
| AlexNet | Custom CNN, trained from scratch |
| VGG16 | ImageNet pretrained, frozen backbone |
| ResNet50 | ImageNet pretrained, frozen backbone |
| EfficientNetB0 | ImageNet pretrained, frozen backbone |

**Compared:** training accuracy, test accuracy, test loss, training time.

---

## Quick map

| Folder | Topic | Dataset | Main stack |
|---|---|---|---|
| Assign 1 | ANN / Keras intro | MNIST | TensorFlow/Keras |
| Assign 2 | MLP | Iris + Wine | scikit-learn |
| Assign 3 | Forward / backprop, LR & epochs | MNIST | TensorFlow/Keras |
| Assign 4 | Simple RNN | IMDB | TensorFlow/Keras |
| Assign 6 | CNN | Leaf disease images | TensorFlow/Keras |
| Assign 7 | Architecture comparison | Pistachio images | TensorFlow/Keras + transfer learning |
