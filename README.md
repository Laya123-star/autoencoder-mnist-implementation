# 🧠 MNIST Autoencoder using Deep Learning

![Python](https://img.shields.io/badge/Python-3.9-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange)
![Autoencoder](https://img.shields.io/badge/Model-Autoencoder-green)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow)

A deep learning project focused on building and evaluating an **Autoencoder Neural Network** for **image reconstruction** using the MNIST handwritten digits dataset.

---

## 🚀 Run Notebook in Google Colab

Click the button below to open the notebook directly in Google Colab.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1HmR5d5TH-Pien5yfwS96sgoFiiFb_DJq)

---

# 📘 Project Overview

This project implements a **basic Autoencoder model** to learn compressed representations of handwritten digit images and reconstruct them.

The project covers the complete deep learning workflow including:

- Dataset loading (MNIST)  
- Data preprocessing and normalization  
- Encoder–Decoder architecture design  
- Model training and validation  
- Loss curve visualization  
- Image reconstruction comparison  

The goal is to build a model that can **efficiently compress and reconstruct image data**.

---

# 🎯 Objective

The main objectives of this project are:

🔹 Understand Autoencoder architecture (Encoder + Decoder)  
🔹 Compress 28×28 images into a latent representation  
🔹 Reconstruct images from compressed features  
🔹 Train and evaluate model performance  
🔹 Visualize reconstruction quality  

---

# 📂 Dataset Information

The dataset used is the **MNIST Handwritten Digits Dataset**.

### Dataset Details

| Feature | Description |
|------|-------------|
| Images | 28×28 grayscale images |
| Classes | Digits (0–9) |
| Training Samples | 60,000 |
| Test Samples | 10,000 |

---

# 🧹 Data Preprocessing

Before training the model, the following preprocessing steps were applied:

### ✔ Normalization
- Pixel values scaled to range **0–1**

### ✔ Reshaping
- Images reshaped into vectors (784) or retained as 28×28

### ✔ Train-Test Split
- Used predefined MNIST training and test datasets

---

# 🧠 Autoencoder Architecture

A **fully connected Autoencoder** was built using **TensorFlow / Keras**.

### Architecture Components

✔ Encoder:
- Dense layers to compress input
- Latent space representation (compressed features)

✔ Decoder:
- Dense layers to reconstruct image
- Output layer with **sigmoid activation**

✔ Loss Function:
- Binary Crossentropy / Mean Squared Error

---

# ⚙ Model Training

The model was trained using the **training dataset** and validated using the **test dataset**.

### Training Details

- Optimizer: Adam  
- Epochs: (as per notebook)  
- Batch Size: (as per notebook)  

Training progress was monitored using:

- Training Loss  
- Validation Loss  

---

# 📊 Model Evaluation

### ✔ Model Summary
- Displays encoder and decoder structure  

### ✔ Loss Curve
- Plotted **training vs validation loss**  
- Shows model learning behavior  

---

# 🖼 Reconstruction Results

The model performance is evaluated by comparing:

- Original images  
- Reconstructed images  

### Observations

- Reconstructed images closely resemble original digits  
- Minor blurring may occur due to compression  
- Model successfully captures key visual features  

---

# 📝 Results Explanation

The autoencoder model successfully learned a compressed representation of the MNIST images and was able to reconstruct them with good accuracy. The training and validation loss decreased steadily, indicating effective learning without major overfitting.

The reconstructed images retain the overall structure and shape of the original digits, although some fine details are slightly blurred. This is expected as the model compresses the image into a lower-dimensional latent space. Overall, the model demonstrates the ability of autoencoders to perform dimensionality reduction and feature learning.

---

# 🛠 Tech Stack

| Tool | Purpose |
|----|----|
| Python | Programming language |
| TensorFlow / Keras | Deep learning framework |
| NumPy | Numerical computation |
| Matplotlib | Visualization |
| Scikit-learn | Preprocessing |
| Google Colab | Development environment |

---

# 📁 Repository Structure

autoencoder-mnist/

│
├── DL_Assignment_3_AutoEncoders.ipynb  
├── README.md  
└── DL Assignment 3 - Auto Encoders.pdf  

---

# 🚀 How to Run the Project

### 1️⃣ Open the Notebook

Click the **Google Colab button above**.

---

### 2️⃣ Install Required Libraries

```python
pip install tensorflow numpy matplotlib scikit-learn

---

## 📌 Academic Submission

This project was created as part of a **Deep Learning assignment**, demonstrating the implementation of an **Autoencoder Neural Network** for image reconstruction using the MNIST dataset. It includes data preprocessing, model design, training, evaluation, and visualization of reconstructed outputs.

---
## ⚠️ Limitations

- The model uses a basic fully connected autoencoder, which may not capture spatial features as effectively as CNN-based autoencoders  

- Reconstruction quality may be slightly blurred due to dimensionality reduction  

- Limited to grayscale images (MNIST dataset only)  

- Does not handle complex or high-resolution image datasets  

- Hyperparameter tuning is minimal and may affect optimal performance  

- Model performance may not generalize well to other image datasets

---

## 📌 Future Enhancements

- Implement **Convolutional Autoencoders (CNN-based)** for better image reconstruction  

- Experiment with **Variational Autoencoders (VAE)**  

- Apply model to more complex datasets (CIFAR-10, medical images, etc.)  

- Perform hyperparameter tuning for improved performance  

- Add noise to input images and build a **Denoising Autoencoder**  

- Deploy the model using a web interface (Streamlit / Flask)  

---

## 👤 Author

**Name:** Laya Mary Joy  

**Organization:** Entri Elevate  

**Date:** March 28, 2026

---

## ⭐ Acknowledgment

Thanks to **Entri Elevate** for guidance and support throughout this project.
