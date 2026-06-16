# Classify Waste Products Using Transfer Learning

This project uses **Transfer Learning with VGG16** to classify waste products into two categories:

- O (Organic Waste)
- R (Recyclable Waste)

The model is built using TensorFlow/Keras and demonstrates both:

1. Feature Extraction
2. Fine-Tuning

as transfer learning techniques for image classification.

---

## 📌 Project Overview

Waste classification is an important step in smart waste management systems. Instead of training a CNN from scratch, this project leverages a pretrained **VGG16** model trained on ImageNet to classify waste images efficiently.

Two transfer learning approaches are implemented:

### 1. Feature Extraction
- Freeze all VGG16 convolutional layers.
- Train only the custom classification layers.

### 2. Fine-Tuning
- Unfreeze selected VGG16 layers.
- Retrain upper convolutional layers along with classifier layers.

---

## 🛠 Technologies Used

- Python
- TensorFlow 2.17
- Keras
- NumPy
- Matplotlib
- Scikit-Learn

---

## 📂 Dataset

Dataset contains two classes:

```text
o-vs-r-split/
│
├── train/
│   ├── O/
│   └── R/
│
└── test/
    ├── O/
    └── R/
