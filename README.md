# 👕 Fashion-MNIST Multi-Class Image Classification using CNN (PyTorch)

This project implements a deep Convolutional Neural Network (CNN) for multi-class image classification using the Fashion-MNIST dataset. The model is built entirely in PyTorch and designed to learn hierarchical image features through multiple convolutional layers.

---

## 📌 Project Objective

The objective of this project is to design and implement a deep CNN architecture consisting of four convolutional blocks, each including:

- Two convolutional layers
- ReLU activation functions
- Batch Normalization
- Max Pooling

The extracted features are then passed through fully connected layers with dropout regularization to perform classification into multiple categories.

---

## 📊 Dataset Description

The dataset used is **Fashion-MNIST (CSV format)**.

Each row represents one image:
- First column → Label (class)
- Remaining 784 columns → Pixel values (28 × 28 grayscale image)

### Image Preprocessing

- Pixel values normalized (0–255 → 0–1)
- Reshaped from:

- Converted into PyTorch tensors for CNN input

---

## 🏷️ Classes

The model classifies images into 10 categories:

| Label | Category |
|------|--------|
| 0 | T-shirt/top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle boot |

---

## 🧠 Model Architecture

The CNN consists of **four convolutional blocks** with increasing depth:

Input: 1 × 28 × 28

Block 1 → 32 filters → Output: 32 × 14 × 14
Block 2 → 64 filters → Output: 64 × 7 × 7
Block 3 → 128 filters → Output: 128 × 3 × 3
Block 4 → 256 filters → Output: 256 × 1 × 1

Flatten → Fully Connected Layers → Output (10 classes)


### Key Components

- **Convolution Layers** → Feature extraction
- **ReLU Activation** → Introduces non-linearity
- **Batch Normalization** → Stabilises and accelerates training
- **Max Pooling** → Reduces spatial dimensions
- **Dropout (0.4)** → Prevents overfitting
- **Fully Connected Layers** → Final classification

---

## ⚙️ Technologies Used

- Python
- PyTorch
- Pandas
- NumPy
- Scikit-learn

---

## 🔄 Workflow

1. Load dataset from CSV file  
2. Split features and labels  
3. Normalize pixel values  
4. Reshape data into image tensors  
5. Train-test split  
6. Create custom PyTorch Dataset  
7. Build CNN model  
8. Train model using CrossEntropyLoss  
9. Evaluate performance using accuracy  

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/your-username/fashion-mnist-cnn-pytorch.git
2. Navigate to the project
cd fashion-mnist-cnn-pytorch
3. Open the notebook
fashion_mnist_cnn_pytorch.ipynb
4. Run all cells in Jupyter Notebook / Kaggle
```
