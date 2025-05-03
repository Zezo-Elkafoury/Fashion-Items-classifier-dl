# 👕 Deep CNN for Fashion Item Classification (Fashion MNIST)

This project implements a **deep Convolutional Neural Network (CNN)** to classify **Fashion MNIST** images into clothing categories (T-shirts, trousers, shoes, bags, etc.).  
The model is built using **TensorFlow/Keras** and follows modern deep learning practices such as **Batch Normalization** and **Dropout** for better accuracy and generalization.

---

## 🚀 Features

- Deep CNN with **6 convolutional layers** (32 ➔ 64 ➔ 128 filters)
- **Batch Normalization** for stable and faster training
- **Dropout** layers to reduce overfitting
- Trained on **28x28 grayscale images**
- **Softmax** output layer for 10 fashion categories

---

## 🏗️ Model Architecture

Input (28x28x1 grayscale image)
│
├── Conv2D(32 filters) + BatchNorm + ReLU
├── Conv2D(32 filters) + BatchNorm + ReLU
├── MaxPooling2D + Dropout(0.25)
│
├── Conv2D(64 filters) + BatchNorm + ReLU
├── Conv2D(64 filters) + BatchNorm + ReLU
├── MaxPooling2D + Dropout(0.25)
│
├── Conv2D(128 filters) + BatchNorm + ReLU
├── Conv2D(128 filters) + BatchNorm + ReLU
├── MaxPooling2D + Dropout(0.25)
│
├── Flatten
├── Dense(128 units) + ReLU + Dropout(0.5)
└── Dense(10 units, Softmax)

## 📊 Results
With proper training (10 epochs), this model achieves:

✅ Training Accuracy: ~92.7%

✅ Test Accuracy: ~92.2%
