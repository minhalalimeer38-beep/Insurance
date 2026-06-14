# 🧠 Artificial Neural Network (ANN) Regression Project

## 📌 Project Title

**Insurance Cost Prediction using Artificial Neural Network (ANN)**

---

## 📊 Project Overview

This project predicts **insurance charges** using a deep learning model (ANN). The dataset contains customer information such as age, gender, BMI, smoking status, and region. The goal is to estimate medical insurance costs based on these features.

The model is built using **TensorFlow/Keras** and uses manual preprocessing with **OneHotEncoder and StandardScaler**.

---

## 📁 Dataset Information

* Dataset: Insurance Dataset
* Target Variable: `charges`
* Input Features:

  * age
  * sex
  * bmi
  * children
  * smoker
  * region

---

## ⚙️ Technologies Used

* Python 🐍
* Pandas & NumPy
* Scikit-learn
* TensorFlow / Keras
* Matplotlib (optional for visualization)

---

## 🔄 Workflow

### 1. Data Loading

* Loaded dataset using pandas

### 2. Data Preprocessing

* Checked missing values
* Checked duplicates

### 3. Feature Engineering

* Split features into:

  * Numerical columns
  * Categorical columns

### 4. Encoding & Scaling

* Categorical → OneHotEncoder (drop='first')
* Numerical → StandardScaler
* Combined using `np.hstack()`

---

## 🧠 Model Architecture (ANN)

* Input Layer → based on processed features
* Hidden Layers:

  * Dense(50, ReLU)
  * Dense(25, ReLU)
  * Dense(15, ReLU)
  * Dense(10, ReLU)
  * Dense(5, ReLU)
* Output Layer:

  * Dense(1, Linear activation)

---

## ⚙️ Model Compilation

* Optimizer: Adam
* Loss Function: Mean Squared Error (MSE)
* Metrics: Mean Absolute Error (MAE)

---

## 🚀 Model Training

* Epochs: 100
* Batch Size: 10
* Validation Split: 20%

---

## 📈 Model Evaluation

The model is evaluated using regression metrics:

* MAE (Mean Absolute Error)
* MSE (Mean Squared Error)
* R² Score

---

## 📊 Results

* MAE: (your output value)
* MSE: (your output value)
* R² Score: **~0.87**

👉 The model explains approximately **87% variance** in insurance charges, which indicates a **good performing regression model**.

---

## 🧠 Key Learnings

* How to preprocess categorical & numerical data separately
* Importance of feature scaling in ANN
* Building deep learning regression model
* Evaluation using regression metrics
* Manual pipeline implementation using NumPy

---

## 📌 Project Highlights

✔ End-to-end ANN regression pipeline
✔ Manual preprocessing (no full sklearn pipeline)
✔ Deep neural network with multiple hidden layers
✔ Good performance (R² ≈ 0.87)
✔ Real-world dataset (Insurance cost prediction)


---

## ▶️ How to Run

```python
python main.py
```

OR run notebook step-by-step.

---

## 🔥 Conclusion

This project demonstrates the use of **Artificial Neural Networks for regression problems** and shows how machine learning can be used to predict real-world insurance costs with good accuracy.

---
