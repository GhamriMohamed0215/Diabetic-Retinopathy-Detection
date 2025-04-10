# Diabetic Retinopathy Detection Using Deep Learning

## 📄 Project Overview

This project aims to detect and classify diabetic retinopathy from retinal fundus images using deep learning techniques. We implemented and compared models such as **AlexNet** and **DenseNet-121** for binary and multi-class classification tasks.


## 🧠 Objectives

- Apply deep learning models to detect diabetic retinopathy (DR).
- Compare model performance in both binary and multi-class classification.
- Use two classification structures:
  - **Binary**: NO DR vs DR
  - **Multi-class**: 5 severity levels

## 🧰 Technologies & Tools

- Python
- TensorFlow / Keras
- Jupyter Notebook
- DenseNet-121, AlexNet
- APTOS 2015 & APTOS 2019 datasets

## 🗃️ Datasets

We used two datasets:

- **APTOS 2019 Blindness Detection**
- **APTOS 2015 Diabetic Retinopathy Detection**

### Preprocessing Steps

- Removed low-quality, blurry, and noisy images
- Applied **Gaussian blur** (sigma=10) to highlight lesions
- Used **circle cropping** to standardize image shapes
- Resized all images to **224x224**
- Performed **data augmentation** (rotation, brightness adjustments) using `ImageDataGenerator`

## ⚙️ Models

### 1. **AlexNet**

A standard CNN used as a baseline model for both binary and multi-class classification.

### 2. **DenseNet-121**

An advanced CNN architecture that achieved the best results:
- **99% accuracy** for binary classification (NO DR vs DR)
- High performance in the 5-class classification task (see notebook for details)

## 📊 Results

| Structure    | Model         | Accuracy |
|--------------|---------------|----------|
| Binary       | DenseNet-121  | 99%      |
| 5 Classes    | DenseNet-121  | High (see notebook) |

Performance comparison, training curves, and confusion matrices are available in the notebook.
