
# 🍷 Wine Classification using KNN

This project demonstrates how to use the **K-Nearest Neighbors (KNN)** algorithm to classify different types of wine based on their chemical properties.

---

## 📌 Project Overview

The goal of this project is to build a classification model that can accurately predict the category of wine using machine learning techniques.

---

## 📊 Dataset

- Dataset: Wine Dataset (from sklearn)
- Number of Classes: 3
- Features include:
  - Alcohol
  - Malic Acid
  - Ash
  - Flavanoids
  - Color Intensity
  - And more...

---

## ⚙️ Workflow

1. **Load Dataset**
   - Used sklearn's built-in wine dataset

2. **Data Preprocessing**
   - Converted dataset into Pandas DataFrame
   - Checked features and target values

3. **Train-Test Split**
   - 70% training data
   - 30% testing data

4. **Feature Scaling**
   - Applied MinMaxScaler (important for KNN)

5. **Model Training**
   - Used KNN with K = 5

6. **Model Evaluation**
   - Accuracy Score
   - Confusion Matrix
   - Classification Report

---

## 📈 Model Performance

### 🔹 Accuracy
**94.4%**
---

### 🔍 Insights

- High accuracy with minimal errors
- Class 0 and Class 2 predicted perfectly
- Slight confusion in Class 1 predictions
- Feature scaling significantly improved performance

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/your-username/your-repo-name.git

# Navigate to folder
cd your-repo-name

# Run Jupyter Notebook
jupyter notebook
