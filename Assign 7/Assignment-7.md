# Assignment 7 — Comparing Deep CNN Architectures

**Aim:** Compare AlexNet, VGG16, ResNet50, and EfficientNetB0 on the same image classification task.

## Concepts
- Transfer learning vs training from scratch
- Frozen pretrained backbones (ImageNet weights)
- AlexNet, VGG16, ResNet50, EfficientNetB0
- ImageNet-style normalization (mean / std)
- Global average pooling vs flatten + dense head
- Dropout
- Trade-off: accuracy vs training time

## Dataset
- **Pistachio Image Dataset** (Kaggle)
- 2 classes: Kirmizi_Pistachio, Siirt_Pistachio
- 2148 images (1719 train, 429 validation)
- Input size: 224×224 RGB
- Batch size: 16

## Tools / Libraries
- TensorFlow / Keras Applications
- kagglehub
- Pandas (comparison table)
- Matplotlib

## Models (high level)
- **AlexNet:** custom CNN, trained from scratch
- **VGG16:** pretrained, frozen; Flatten + Dense 4096 + Dropout
- **ResNet50:** pretrained, frozen; GlobalAveragePooling + Softmax
- **EfficientNetB0:** pretrained, frozen; GlobalAveragePooling + Dropout + Softmax
- All: Adam (lr 0.001), sparse categorical cross-entropy, 10 epochs

## Metrics
- Training accuracy
- Test / validation accuracy
- Test loss
- Training time (minutes)
