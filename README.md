# 💰 Deep Learning Based Fake Currency Detection

##  Project Title
Fake Currency Detection using Deep Learning (CNN and MobileNetV2)

---

##  Problem Statement

Counterfeit currency poses a major threat to financial systems and economies around the world. Detecting fake currency manually requires expertise and specialized equipment. Therefore, an automated system that can identify counterfeit currency using image analysis is highly desirable.

The objective of this project is to develop a **deep learning-based system** capable of classifying currency notes as **real or fake** using image classification techniques.

---

##  Project Explanation

This project uses **Deep Learning models** to detect counterfeit currency notes from images.

### Project Workflow

1. **Dataset Collection**
   - Images of real and fake Indian currency notes were collected.

2. **Data Preprocessing**
   - Images were resized to a fixed dimension (224×224).
   - Pixel values were normalized.
   - Data augmentation techniques such as rotation, zooming, and brightness adjustment were applied to improve model performance.

3. **Model Development**

Two deep learning techniques were used:

### 1️⃣ Convolutional Neural Network (CNN)

A custom CNN architecture was built to automatically extract visual features from currency images.

The CNN consists of:
- Convolutional layers
- Max pooling layers
- Fully connected layers
- Sigmoid activation for binary classification

The model learns patterns that distinguish **real currency notes from counterfeit ones**.

---

### 2️⃣ Transfer Learning using MobileNetV2

To improve performance, **transfer learning** was implemented using the pretrained MobileNetV2 architecture.

Steps performed:
- Load pretrained MobileNetV2 without the top classification layer
- Freeze the base layers
- Add custom dense layers
- Train the model on the currency dataset

Transfer learning helps leverage features learned from large image datasets.

---

##  Model Evaluation

The models were evaluated using the following metrics:

- Accuracy
- Confusion Matrix
- Classification Report

These metrics help measure how well the model distinguishes between **real and fake currency notes**.

---

## 📂 Dataset

The dataset contains images of **real and fake Indian currency notes**.

Dataset Source:  
https://github.com/prernarohra/Fake-Currency-Checker

### Dataset Structure

```
Indian Currency Dataset/
│
├── train/
│   ├── real/
│   └── fake/
│
├── validation/
│   ├── real/
│   └── fake/
│
└── test/
    ├── real/
    └── fake/
```

##  Technologies Used

- Python  
- TensorFlow  
- Keras  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Google Colab  

---

## ⚙️ How to Run the Project

1. Clone the repository

git clone https://github.com/your-username/fake-currency-detection.git

2. Install required libraries

pip install tensorflow keras numpy matplotlib seaborn scikit-learn

3. Open the notebook in **Google Colab or Jupyter Notebook**

4. Run all cells to train and evaluate the models.

---

##  Project Outcome

The deep learning models successfully learned to classify currency images as **real or fake**.  
This project demonstrates how deep learning techniques can be used to automate counterfeit currency detection.

---

##  Project Video

An explanation video (8–10 minutes) demonstrating the working of the project is included in the submission.

---

##  Author

Chhavi Sharma  
B.Tech Student – Deep Learning Project
