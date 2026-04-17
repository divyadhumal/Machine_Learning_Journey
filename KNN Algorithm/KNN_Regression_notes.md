
# 🏡 California Housing Price Prediction using KNN

## 📌 Project Overview
In this project, I used the K-Nearest Neighbors (KNN) Regression algorithm to predict housing prices based on different features like income, location, and population.

This project helped me understand how machine learning models work with real-world datasets.

---

## 📊 Dataset
- Dataset: California Housing Dataset (from sklearn)
- Features include:
  - Median Income
  - House Age
  - Population
  - Location (Latitude, Longitude)

---

## ⚙️ Steps Performed

1. Loaded the dataset using sklearn
2. Split data into training and testing sets
3. Applied **MinMax Scaling** (important for KNN)
4. Trained KNN Regressor model (k=5)
5. Made predictions on test data
6. Evaluated model using:
   - RMSE (Root Mean Squared Error)
   - R² Score

---

## 📈 Results

- RMSE:  0.62487511
- R² Score:  0.7025089

---

## 🧠 Key Learnings

- KNN works based on distance between data points
- Scaling is very important for KNN
- Model performance depends on value of K
- RMSE helps measure prediction error

---

## 🚀 Future Improvements

- Try different values of K
- Compare with other models (Linear Regression, Decision Tree)
- Visualize results

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn

---

## 📎 Author
Divya Dhumal
