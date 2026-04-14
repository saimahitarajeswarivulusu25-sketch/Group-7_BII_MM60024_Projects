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

  

## 🧠 Technologies Used
- Python
- TensorFlow / Keras
- DenseNet121
- NumPy, Matplotlib, Seaborn
- Scikit-learn

---

## 📌 Notes
- This project is developed as part of **Biomedical Imaging Informatics (MM60024)** coursework by group 7
- **22BT30022 Rahul Choudhary**
  
**22BT30030 Supratim Sarkar**
  
**22BT30009 Banoth Arun**

  **25MM61R16 Aman Kumar**
  
**25MM61R03 Sai Mahitha Rajeswari Vulusu**
- The model can be further improved using fine-tuning and larger datasets.

