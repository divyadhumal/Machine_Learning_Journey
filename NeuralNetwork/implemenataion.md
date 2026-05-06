## Code Explanation (Step by Step)

### 1. Import Libraries

```python
import numpy as np
import matplotlib.pyplot as plt
```

**Explanation:**

* `numpy` is used for numerical operations (arrays, matrix multiplication)
* `matplotlib` is used for visualization

---

### 2. Initialize Weights and Biases

```python
W = np.random.randn(input_size, hidden_size)
b = np.zeros((1, hidden_size))
```

**Explanation:**

* We initialize weights randomly so the model can learn different patterns
* Bias is initialized as zero
* Shape depends on number of input features and neurons

---

### 3. Define Activation Function

```python
def relu(x):
    return np.maximum(0, x)
```

**Explanation:**

* ReLU replaces negative values with 0
* Helps introduce non-linearity

---

### 4. Forward Propagation

```python
Z1 = np.dot(X, W) + b
A1 = relu(Z1)
```

**Explanation:**

* `np.dot(X, W)` → multiplies input with weights
* `+ b` → adds bias
* `relu()` → applies activation function
* This produces output of the hidden layer

---

### 5. Output Layer Calculation

```python
Z2 = np.dot(A1, W2) + b2
```

**Explanation:**

* Takes hidden layer output as input
* Produces final prediction

---

### 6. Loss Calculation

```python
loss = np.mean((y_pred - y_true) ** 2)
```

**Explanation:**

* Measures error between predicted and actual values
* Lower loss = better model

---

### 7.  Backpropagation Concept

```python
# gradient calculation (if implemented)
```

**Explanation:**

* Used to update weights
* Helps reduce loss over time

---

## Summary of Flow

1. Input →
2. Multiply with weights →
3. Add bias →
4. Apply activation →
5. Repeat for layers →
6. Get output

---

## Note

This implementation is for learning purposes to understand how neural networks work internally.
