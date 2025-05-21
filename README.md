# Sonar Signal Classification using CNN and GAN (WIP)

This project focuses on classifying sonar signals into underwater object types — **fish**, **mine**, and **rock** — by converting raw sonar signals into **spectrogram images** and processing them using a **Convolutional Neural Network (CNN)**.

> ⚠️ **Note:** GAN-based synthetic data generation is a **work in progress**. The current results are based on simulated data. Future commits will integrate GAN pipelines for augmenting sonar spectrogram datasets.

---

## 🔍 Problem Statement

Sonar datasets are often limited in size and diversity, which impacts classification performance. This project aims to:
- Simulate and generate sonar signals
- Convert signals into spectrogram images
- (WIP) Augment data using **GAN**
- Train a CNN model for classification

---

## 🧠 Technologies Used

- **Python**
- **TensorFlow / Keras**
- **NumPy**, **Matplotlib**, **Scipy**
- **PIL** for image handling
- **CNN (Convolutional Neural Network)**
- **GAN (WIP)** for future augmentation
- **Spectrograms** for visual representation

---

## 🧱 Model Architectures

### 🧩 CNN
- 3x Conv2D + ReLU + MaxPooling
- Flatten → Dense → Dropout → Softmax

### 🧩 GAN *(Work in Progress)*
- Generator: Converts noise → fake sonar spectrogram
- Discriminator: Distinguishes real vs. generated images
- Will be used to improve training data variety

---

## Results

Achieved **~100% training and validation accuracy** on synthetic data within 10 epochs — demonstrating the effectiveness of spectrogram + CNN pipeline.

---

## 🧪 Future Work

- Finish GAN implementation & integrate synthetic spectrograms
- Experiment with **CycleGAN** for real-synthetic domain bridging
- Anomaly detection in sonar time series
---

## How to Run

```bash
# Clone the repo
git clone https://github.com/tejonish/sonar_classification.git

# Open in Google Colab
Upload your notebook or run from the provided .ipynb
