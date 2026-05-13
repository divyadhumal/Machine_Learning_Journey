 # Anomaly Detection using Isolation Forest

## Overview
This project demonstrates how to detect anomalies (unusual data points) using the **Isolation Forest Algorithm** in Machine Learning.

The model identifies transactions that behave differently from normal patterns and marks them as anomalies.

---

## Objective
The main goal of this project is to:
- Detect unusual transactions
- Understand anomaly detection concepts
- Visualize anomalies using plots
- Learn unsupervised machine learning techniques

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Algorithm Used
## Isolation Forest

Isolation Forest is an unsupervised learning algorithm used for anomaly detection.

It works by:
- Randomly selecting features
- Randomly splitting data points
- Isolating anomalies faster than normal points

Anomalies are easier to isolate because they are rare and different from normal observations.

---

## Project Workflow

### 1. Import Required Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.ensemble import IsolationForest
from sklearn.preprocessing import StandardScaler
```

---

### 2. Load Dataset

```python
df = pd.read_csv("creditcard.csv")
```

---

### 3. Data Preprocessing
- Checked missing values
- Scaled transaction amount using `StandardScaler`

```python
scaler = StandardScaler()
df['scaled_amount'] = scaler.fit_transform(df[['Amount']])
```

---

### 4. Feature Selection

```python
features = ['scaled_amount', 'Time'] + [f'V{i}' for i in range(1,29)]
X = df[features]
```

---

### 5. Train Isolation Forest Model

```python
model = IsolationForest(
    n_estimators=100,
    contamination=0.001,
    random_state=42
)
```

---

### 6. Detect Anomalies

```python
df['anomaly'] = model.fit_predict(X)
```

Output:
- `1` → Normal Transaction
- `-1` → Anomaly / Fraud

---

### 7. Generate Anomaly Scores

```python
df['anomaly_score'] = model.decision_function(X)
```

---

## Data Visualization

### Scatter Plot
Visualized:
- Normal transactions
- Fraudulent transactions
- Transaction amount vs time

### Histogram
Visualized anomaly score distribution.

---

## Results
- Successfully detected unusual transactions
- Understood how anomaly detection works
- Learned visualization of anomalies

---

## Key Learnings
- Unsupervised Machine Learning
- Isolation Forest Algorithm
- Feature Scaling
- Anomaly Detection
- Data Visualization

---

## Future Improvements
- Hyperparameter tuning
- Compare with Local Outlier Factor
- Evaluate using precision and recall
- Deploy using Streamlit

 

 

