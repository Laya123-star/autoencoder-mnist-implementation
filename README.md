# 🧠 MNIST Autoencoder using Deep Learning

![Python](https://img.shields.io/badge/Python-3.9-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange)
![Autoencoder](https://img.shields.io/badge/Model-Autoencoder-green)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow)

A deep learning project that focuses on building and evaluating an **Autoencoder Neural Network** for **image reconstruction** using the MNIST handwritten digits dataset.

---

## 🚀 Run Notebook in Google Colab

Click below to open the notebook directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1HmR5d5TH-Pien5yfwS96sgoFiiFb_DJq)

---

## 📘 Project Overview

This project demonstrates how an **Autoencoder model** can learn compressed representations of image data and reconstruct the original images.

The workflow includes:

- Loading the MNIST dataset
  
- Data preprocessing and normalization
  
- Designing encoder–decoder architecture
  
- Training and validating the model
  
- Visualizing loss curves
  
- Comparing original and reconstructed images  

The primary goal is to build a model capable of **efficient data compression and accurate image reconstruction**.

---

## 🎯 Objective

- Understand the working of Autoencoders (Encoder + Decoder)
   
- Compress 28×28 images into a lower-dimensional latent space
  
- Reconstruct images from compressed representations
  
- Evaluate reconstruction performance
  
- Visualize and interpret output quality  

---

## 📂 Dataset Information

The dataset used is the **MNIST Handwritten Digits Dataset**.

### Dataset Details

| Feature | Description |
|--------|------------|
| Images | 28×28 grayscale images |
| Classes | Digits (0–9) |
| Training Samples | 60,000 |
| Test Samples | 10,000 |

---

## 🧹 Data Preprocessing

The following preprocessing steps were applied:

### ✔ Normalization
- Pixel values scaled to the range **0–1**

### ✔ Reshaping
- Images reshaped into vectors (784) or maintained as 28×28 format

### ✔ Train-Test Split
- Used predefined MNIST training and test datasets

---

## 🧠 Autoencoder Architecture

A **fully connected Autoencoder** was implemented using **TensorFlow / Keras**.

### Architecture Components

✔ **Encoder**
- Dense layers to compress input data
  
- Generates a compact latent representation  

✔ **Decoder**
- Dense layers to reconstruct the image
  
- Output layer uses **sigmoid activation**  

✔ **Loss Function**
- Binary Crossentropy / Mean Squared Error  

---

## ⚙ Model Training

The model was trained using the training dataset and evaluated on the test dataset.

### Training Details

- Optimizer: Adam
  
- Epochs: (as defined in notebook)
  
- Batch Size: (as defined in notebook)  

### Monitoring

- Training Loss
  
- Validation Loss  

---

## 📊 Model Evaluation

### ✔ Model Summary
- Displays encoder and decoder architecture  

### ✔ Loss Curve
- Visual comparison of training vs validation loss
  
- Helps identify learning trends and overfitting  

---

## 🖼 Reconstruction Results

Model performance is evaluated by comparing:

- Original images
  
- Reconstructed images  

### Observations

- Reconstructed images closely resemble the original digits
  
- Slight blurring occurs due to compression

- Key visual features are preserved effectively  

---

## 📝 Results Explanation

The autoencoder successfully learned meaningful compressed representations of the MNIST dataset. Both training and validation loss decreased steadily, indicating stable learning.

Although reconstructed images may lose some fine details, the overall structure and digit shapes are preserved. This demonstrates the effectiveness of autoencoders in **dimensionality reduction and feature learning**.

---

## 🛠 Tech Stack

| Tool | Purpose |
|------|--------|
| Python | Programming language |
| TensorFlow / Keras | Deep learning framework |
| NumPy | Numerical computation |
| Matplotlib | Visualization |
| Scikit-learn | Preprocessing |
| Google Colab | Development environment |

---

## 📁 Repository Structure

```
autoencoder-mnist/

│

├── DL_Assignment_3_AutoEncoders.ipynb

├── README.md

└── DL Assignment 3 - Auto Encoders.pdf
```

---

## 🚀 How to Run the Project

### 1️⃣ Open the Notebook
Click the **Google Colab button above**

---

### 2️⃣ Install Required Libraries

```bash
pip install tensorflow numpy matplotlib scikit-learn
```

---

### 3️⃣ Run the Notebook

- Execute all cells step-by-step
  
- Train the model
  
- Visualize reconstruction results  

---

## 📌 Academic Submission

This project was developed as part of a **Deep Learning assignment**, demonstrating the implementation of an **Autoencoder Neural Network** for image reconstruction. It covers data preprocessing, model design, training, evaluation, and visualization.

---

## ⚠️ Limitations

- Uses a basic fully connected architecture instead of CNN-based models
  
- Reconstruction may appear slightly blurred due to compression
  
- Limited to grayscale MNIST dataset
  
- Not suitable for complex or high-resolution images
  
- Minimal hyperparameter tuning
  
- Limited generalization to other datasets  

---

## 📌 Future Enhancements

- Implement **Convolutional Autoencoders (CNN-based)**
  
- Explore **Variational Autoencoders (VAE)**
  
- Apply to complex datasets like CIFAR-10
  
- Perform advanced hyperparameter tuning
  
- Build a **Denoising Autoencoder**
  
- Deploy using **Streamlit / Flask**  

---

## 👤 Author

**Name:** Laya Mary Joy  

**Organization:** Entri Elevate  

**Date:** March 28, 2026  

---

## ⭐ Acknowledgment

I would like to thank **Entri Elevate** for their valuable guidance and support throughout this project.

---
