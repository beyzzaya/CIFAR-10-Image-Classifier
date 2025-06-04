# CIFAR-10-Image-Classifier

This repository contains **`CIFAR-10-Image-Classifier.ipynb`**, a self-contained Jupyter Notebook that
trains a Convolutional Neural Network (CNN) to classify images in the
**CIFAR-10** dataset (airplane, car, bird, cat, deer, dog, frog, horse, ship,
truck).

### Highlights
- **Data pipeline** — downloads CIFAR-10 via Keras, normalises pixel values,
  adds random horizontal flip & slight rotation for augmentation.
- **Model** — 3 convolutional blocks  
  (`Conv2D → ReLU → Conv2D → ReLU → MaxPool`) followed by
  `Flatten → Dense(256) → Dropout → Dense(10, softmax)`.
- **Training** — Adam optimiser, categorical cross-entropy, 30 epochs.
- **Result** — reaches **≈ 75 % validation accuracy** by epoch 25  

