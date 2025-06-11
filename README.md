# 🧠 Lung and Colon Cancer Detection using CNN 🩸
![Screenshot 2025-02-26 220506](https://github.com/user-attachments/assets/9f98caeb-2a27-4fad-953c-207c6d45bfc7)
![Screenshot 2025-02-26 222512](https://github.com/user-attachments/assets/645e45af-b4ec-474f-acbf-0c5eae1f1031)
![Screenshot 2025-02-26 221445](https://github.com/user-attachments/assets/ffcebce6-8f73-4d87-9a19-87459ddbec9a)


## 🧬 Project Overview

Lung and colon cancers are among the deadliest and most common forms of cancer globally. Early detection significantly increases survival rates—but traditional diagnostic methods are labor-intensive and error-prone.

This project harnesses the power of **Convolutional Neural Networks (CNNs)** and medical image processing to automatically classify histopathological images into **benign or malignant** categories for **lung** and **colon** tissue samples.

> ⚕️ Powered by deep learning, this model aids pathologists in making faster, more accurate diagnoses.

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `coloncancer.ipynb` | Jupyter Notebook containing the full model pipeline—from loading histopathology images to classification using CNNs. |
| `Lung and colon cancer.docm` | Complete documentation with problem statement, architecture, results, and conclusion. |
| `README.md` | This file: detailed overview of the project and how to run it. |

---

## 📷 Dataset Description

The dataset includes histopathological image slides of **lung** and **colon** tissues. Each image is labeled as:

- **Benign** (non-cancerous)
- **Malignant** (cancerous)

### 🔍 Sample Categories:
- **Lung_Adenocarcinoma**
- **Lung_Squamous_Cell_Carcinoma**
- **Colon_Adenocarcinoma**
- **Colon_Benign_Tissue**

---

## 🧠 Model Architecture

This project uses a custom CNN architecture built from scratch with the following layers:

- Convolutional Layers with ReLU activation
- MaxPooling Layers for spatial reduction
- Fully Connected Dense Layers
- Softmax Output Layer for classification

<p align="center">
  <img src="images/cnn_architecture.png" alt="CNN Model" width="600"/>
</p>

The model is trained using **categorical cross-entropy loss**, **Adam optimizer**, and evaluated using **accuracy**, **confusion matrix**, and **classification report**.

---

## 📊 Performance

After training on lung and colon cancer images, the model achieved:

| Tissue Type | Accuracy |
|-------------|----------|
| Lung | 97.6% |
| Colon | 98.3% |
| Combined | 98.0% |

Confusion matrices, training plots, and sample predictions are available in the notebook for visual insight.

<p align="center">
  <img src="images/confusion_matrix_colon.png" alt="Confusion Matrix Colon" width="400"/>
  <img src="images/confusion_matrix_lung.png" alt="Confusion Matrix Lung" width="400"/>
</p>

---

## 🛠️ How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/lung-colon-cancer-cnn.git
cd lung-colon-cancer-cnn
