# Pneumonia Detection Using Chest X-ray Images

## 📌 Project Overview
This project focuses on detecting pneumonia from chest X-ray images using deep learning. Pneumonia is a serious lung infection, and early detection can help in timely treatment. This model automates the diagnosis process using image classification techniques.

---

## 🎯 Objective
- To classify chest X-ray images into:
  - **Normal**
  - **Pneumonia**
- To build a reliable deep learning model using transfer learning.

---

## 📂 Dataset
- Dataset: Chest X-ray Pneumonia Dataset
- Contains:
  - Training set
  - Validation set
  - Test set
- Classes:
  - Normal
  - Pneumonia

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Image resizing to **224 × 224**
- Normalization (rescaling pixel values)
- Data augmentation:
  - Rotation
  - Zoom
  - Horizontal flipping

### 2. Model Architecture
- Base Model: **DenseNet121 (pre-trained on ImageNet)**
- Custom Layers:
  - Global Average Pooling
  - Batch Normalization
  - Dense Layer (ReLU)
  - Dropout (0.5)
  - Output Layer (Sigmoid)

### 3. Training
- Loss Function: Binary Crossentropy
- Optimizer: Adam
- Epochs: 30
- Batch Size: 32

---

## 📊 Results
- Model evaluated on test dataset
- Metrics used:
  - Accuracy
  - F1-score
  - Confusion Matrix
- The model performs well in distinguishing between normal and pneumonia cases.

---

## 📈 Output Visualization
- Confusion Matrix plotted using Seaborn
- Classification report generated
- Prediction on custom uploaded images supported

---

## ▶️ How to Run

1. Open the notebook in **Google Colab**
2. Mount Google Drive
3. Upload or link dataset (train, val, test folders)
4. Run all cells sequentially
5. Upload an X-ray image to test predictions

---

## 💾 Model Saving
- Best model is saved automatically using ModelCheckpoint
- File saved as:
