# **QR Code Classification**

## **📌 Project Overview**
QR codes are widely used for authentication and verification. However, counterfeit QR codes pose a security risk. This project aims to develop a classification model to distinguish **original QR codes** from **counterfeit ones** using **machine learning (SVM, Random Forest)** and **deep learning (CNN, ResNet50)** approaches.

## **📂 Dataset**
- **Total Images**: 200 (100 original, 100 counterfeit)
- **Classes**:
  - **First Prints**: Original QR codes.
  - **Second Prints**: Counterfeit QR codes (scanned and reprinted versions).
- **Preprocessing**:
  - Resized to 128x128 (CNN) and 224x224 (ResNet50).
  - Normalization & Data Augmentation (rotation, zoom, flipping, etc.).

## **📊 Models Used**
### **1️⃣ Traditional Machine Learning Models**
✅ **Feature Extraction**: Brightness, Contrast, Edge Density, Sharpness, Texture Features.  
✅ **Algorithms**:
- Support Vector Machine (SVM) - **Accuracy: 97.5%**
- Random Forest - **Accuracy: 97.5%**

### **2️⃣ Deep Learning Models**
✅ **Custom CNN**: 2 Conv layers, MaxPooling, Dropout.  
- **Initial CNN Accuracy**: **85% (Training), 60% (Test Predictions)**

### **🔹 Running the Code**
1. Clone the repository:
```bash
git clone https://github.com/your-repo/QR-classification.git
cd QR-classification
```
2. Run the Jupyter Notebook:
```bash
jupyter notebook qr-code-assignmnet.ipynb
```

## **🚀 Deployment Considerations**
- **Computational Efficiency**:
  - CNN model is lightweight and can run on edge devices.
  - ResNet50 requires GPU for optimal performance.
- **Robustness to Different Conditions**:
  - Handling low-quality scans using data augmentation.
  - Model generalization tested on varying lighting conditions.
- **Security Implications**:
  - Risk of adversarial attacks (altered QR codes).
  - Solution: Use additional security layers like cryptographic signatures.

## **📌 Future Improvements**
🔹 Increase dataset diversity.
🔹 Explore Vision Transformers for better feature extraction.
🔹 Deploy model as a real-time authentication API.

---
**🔗 Author: Siddharth Upadhyay | Date: 25-03-25**

