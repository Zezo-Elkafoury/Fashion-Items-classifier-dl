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

Input: (28 x 28 x 1) grayscale image

Layer 1: Conv2D (32 filters, 3x3) + BatchNorm + ReLU
Layer 2: Conv2D (32 filters, 3x3) + BatchNorm + ReLU
Layer 3: MaxPooling2D (2x2) + Dropout (0.25)

Layer 4: Conv2D (64 filters, 3x3) + BatchNorm + ReLU
Layer 5: Conv2D (64 filters, 3x3) + BatchNorm + ReLU
Layer 6: MaxPooling2D (2x2) + Dropout (0.25)

Layer 7: Conv2D (128 filters, 3x3) + BatchNorm + ReLU
Layer 8: Conv2D (128 filters, 3x3) + BatchNorm + ReLU
Layer 9: MaxPooling2D (2x2) + Dropout (0.25)

Layer 10: Flatten
Layer 11: Dense (128 units) + ReLU + Dropout (0.5)
Layer 12: Dense (10 units) + Softmax

## 📊 Results
With proper training (10 epochs), this model achieves:

✅ Training Accuracy: ~92.7%

✅ Test Accuracy: ~92.2%
