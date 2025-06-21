
# 📊 NumPy Essentials

> NumPy (Numerical Python) is the foundational library for numerical computing in Python. It provides fast and efficient array operations and forms the base for libraries like Pandas, SciPy, and scikit-learn.

---

## 📦 1. Installation
```bash
pip install numpy
```

---

## 🧠 2. Key Concepts

| Concept             | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| ndarray             | Core data structure in NumPy — N-dimensional array                          |
| Vectorization       | Avoids Python loops using array-wise operations                            |
| Broadcasting        | Automatic expansion of arrays to match shape for operations                |
| Universal Functions | (`ufuncs`) Element-wise operations like `np.add`, `np.sqrt`                 |
| Memory Efficiency   | Arrays use contiguous memory blocks for faster computation                  |

---

## 🧱 3. Creating Arrays

```python
import numpy as np

a = np.array([1, 2, 3])              # 1D array
b = np.array([[1, 2], [3, 4]])       # 2D array

np.zeros((2, 3))                     # Matrix of zeros
np.ones((3, 3))                      # Matrix of ones
np.full((2, 2), 7)                   # Matrix filled with 7
np.eye(3)                            # Identity matrix
np.arange(0, 10, 2)                  # [0, 2, 4, 6, 8]
np.linspace(0, 1, 5)                 # 5 points between 0 and 1
```

---

## 🧪 4. Array Attributes

```python
a.shape           # Dimensions (rows, cols)
a.ndim            # Number of dimensions
a.size            # Total number of elements
a.dtype           # Data type of elements
a.itemsize        # Size of each element (bytes)
```

---

## 🧮 5. Indexing & Slicing

```python
a[0]              # First element
a[-1]             # Last element
a[1:3]            # Slice
a[:, 1]           # All rows, 2nd column
a[1, :]           # 2nd row, all columns
a[::2]            # Every second element
```

---

## 🔁 6. Array Operations

```python
a + b             # Element-wise addition
a - b             # Subtraction
a * b             # Element-wise multiplication
a / b             # Division
a @ b             # Matrix multiplication
np.dot(a, b)      # Matrix multiplication
```

### Aggregation Functions:
```python
np.sum(a)
np.mean(a)
np.std(a)
np.min(a)
np.max(a)
np.argmin(a)
np.argmax(a)
```

---

## 🔄 7. Reshaping & Manipulation

```python
a.reshape((2, 3))     # Reshape
a.flatten()           # Flatten to 1D
np.concatenate([a, b], axis=0)
np.vstack([a, b])     # Vertical stack
np.hstack([a, b])     # Horizontal stack
a.T                   # Transpose
np.split(a, 2)        # Split array
```

---

## 🎭 8. Boolean Masking & Filtering

```python
a > 3                     # Boolean array
a[a > 3]                  # Filtered elements
np.where(a > 3, 1, 0)     # Replace conditionally
```

---

## 🧮 9. Random in NumPy

```python
np.random.seed(42)               # Set seed
np.random.rand(2, 2)             # Uniform [0,1)
np.random.randn(3)               # Standard normal
np.random.randint(1, 10, 5)      # Random integers
np.random.choice([1, 2, 3], 2)   # Random choice
```

---

## 🧹 10. Useful Tips

| Tip                             | Code Example                          |
|----------------------------------|----------------------------------------|
| Check NaN                       | `np.isnan(a)`                         |
| Replace NaN                     | `np.nan_to_num(a)`                    |
| Element-wise comparison         | `np.array_equal(a, b)`                |
| Copy vs View                    | `b = a.copy()` (deep copy)            |

---

## 🧮 11. Linear Algebra (Bonus)

```python
np.linalg.inv(a)           # Inverse
np.linalg.det(a)           # Determinant
np.linalg.eig(a)           # Eigenvalues & Eigenvectors
np.linalg.solve(A, b)      # Solve Ax = b
```

---

## 📘 12. Recommended Practice

- [NumPy Quickstart Tutorial](https://numpy.org/doc/stable/user/quickstart.html)
- [Kaggle NumPy Exercises](https://www.kaggle.com/code/ashishpatel26/numpy-100-basic-exercises)
