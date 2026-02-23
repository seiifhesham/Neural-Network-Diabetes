# Neural Network for Diabetes Prediction  
## Pima Indians Diabetes Dataset

This repository contains a neural network–based binary classification project applied to the **Pima Indians Diabetes** dataset.  
The project demonstrates how the same deep learning pipeline used in the lab can be generalized to a new medical dataset.

---

## 📌 Problem Description

The goal is to predict whether a patient has diabetes based on eight clinical features such as glucose level, blood pressure, BMI, insulin, and age.

- **Type**: Binary classification  
- **Target variable**: `Outcome`
  - `0` → No Diabetes  
  - `1` → Diabetes  

---

## 📊 Dataset

- **Source (Kaggle – UCI ML Repository mirror):**  
  https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

The dataset contains medical diagnostic measurements for Pima Indian women and is known to be challenging and noisy, making it suitable for evaluating model generalization.

---

## ⚙️ Methodology

The project follows a complete neural network workflow:

1. Data loading and exploration  
2. Data preprocessing  
   - Handling invalid zero values  
   - Feature standardization  
3. Baseline neural network implementation  
4. Modified architecture with dropout regularization  
5. Training with early stopping  
6. Evaluation using accuracy, precision, recall, F1-score, and confusion matrix  

---

## 🧠 Model Architecture

**Model:**

```
Input(8) → Dense(64, ReLU) → Dropout(0.3)
        → Dense(32, ReLU) → Dropout(0.2)
        → Dense(16, ReLU) → Output(1, Sigmoid)
```

Dropout and early stopping were used to reduce overfitting and improve generalization.

---

## 📈 Results

- **Test Accuracy**: ~74.7%  
- Performance falls within the expected **70–75% range** for this dataset  
- Training and validation curves show stable convergence  
- Confusion matrix indicates balanced classification behavior  

---

## 📝 Notes

- The focus of this project is generalization and correct evaluation, not achieving unrealistically high accuracy.
- Emphasis is placed on medical interpretation of errors and overfitting control.

---

## 👤 Author

**Seif Hesham**  
Faculty of Engineering – Cairo University (CUFE)
