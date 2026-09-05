# NumPy

This folder contains my learning and practice of **NumPy**, one of the fundamental Python libraries used in Data Science, Machine Learning, and AI.

NumPy provides powerful tools for working with **arrays, vectors, matrices, numerical operations, and mathematical computations**.

---

## 📂 Folder Structure

```text
NumPy/
│
├── Arrays.ipynb
├── array_indexing.ipynb
├── array_operations.ipynb
├── exersises.ipynb
│
└── README.md
```

---

## 📚 Topics Covered

### 1. Basic Array Creation

File: `Arrays.ipynb`

Learned how to create NumPy arrays from Python lists.

```python
import numpy as np

arr = np.array([1, 2, 3, 4])
```

Covered:

* Creating 1D arrays
* Creating 2D arrays
* Converting Python lists into NumPy arrays
* Working with vectors and matrices

---

### 2. Array Generation Functions

File: `Arrays.ipynb`

Covered NumPy functions for generating arrays:

* `np.arange()`
* `np.zeros()`
* `np.ones()`
* `np.linspace()`

Examples:

```python
np.arange(1, 11, 2)

np.zeros((4, 8))

np.ones((6, 6))

np.linspace(0, 1, 100)
```

---

### 3. Random Array Generation

File: `Arrays.ipynb`

Learned basic random-number generation using:

* `np.random.rand()`
* `np.random.randn()`
* `np.random.randint()`

Examples:

```python
np.random.rand(10)

np.random.randn(10)

np.random.randint(10, 20, 10)
```

---

### 4. Array Attributes

File: `Arrays.ipynb`

Learned important NumPy array attributes:

* `shape`
* `size`
* `dtype`

Example:

```python
arr.shape
arr.size
arr.dtype
```

These attributes help understand the structure and data type of an array.

---

### 5. Array Methods

File: `Arrays.ipynb`

Practiced numerical methods such as:

* `min()`
* `max()`
* `sum()`
* `mean()`
* `std()`
* `argmax()`
* `argmin()`

Also practiced `axis` with `np.sum()`:

```python
np.sum(arr, axis=1)
np.sum(arr, axis=0)
```

Here:

```text
axis=1 → row-wise operation
axis=0 → column-wise operation
```

---

### 6. Reshaping Arrays

File: `Arrays.ipynb`

Learned how to change the structure of an array using:

```python
arr.reshape(6, 5)
```

Practiced converting a 1D array into a matrix.

---

# 🔍 Array Indexing and Slicing

File: `array_indexing.ipynb`

This notebook focuses on accessing and extracting data from NumPy arrays.

---

## Vector Indexing

Practiced:

```python
arr[4]
```

---

## Vector Slicing

Covered:

```python
arr[0:5]

arr[4:]

arr[3::2]
```

Concepts:

* Starting index
* Ending index
* Step
* Partial slicing

---

## Matrix Indexing

Practiced accessing individual elements:

```python
arr[4, 3]
```

Also explored:

```python
arr[4][3]
```

---

## Matrix Row Selection

Practiced selecting rows:

```python
arr[0]
arr[3]
```

---

## Matrix Slicing

Practiced extracting sections of matrices:

```python
arr[2:5, 2:4]

arr[2:5, 2:]

arr[3:, 3:]
```

---

## Column Selection

Practiced selecting a complete column:

```python
arr[:, 4]
```

---

# 🟦 Boolean Indexing

File: `array_indexing.ipynb`

Learned how Boolean conditions can be used to filter NumPy arrays.

Example:

```python
bool_index = arr % 2 == 0

arr2 = arr[bool_index]
```

This was practiced to extract elements based on a condition.

---

# ⚙️ Array Operations

File: `array_operations.ipynb`

Learned numerical operations between NumPy arrays.

---

## Arithmetic Operations

Practiced:

```python
a1 + a2
a1 - a2
a1 * a2
a1 / a2
a1 // a2
a1 ** a2
```

Also learned that operations can create a **new array without changing the original arrays**.

---

## Broadcasting

Learned how NumPy can perform operations between an array and a single value.

Example:

```python
arr + 10
arr - 10
```

Also practiced broadcasting with 2D arrays:

```python
arr2 + 10
```

---

# 📋 Copying Arrays

File: `array_operations.ipynb`

Practiced the difference between:

### Reference

```python
b = a
```

Here `b` refers to the same array.

### Copy

```python
b = a.copy()
```

Here a separate copy of the array is created.

This notebook also explores array slicing and how modifying references/copies affects the original array.

---

# ➗ Matrix Operations

File: `array_operations.ipynb`

Practiced operations between matrices:

```python
A + B
A - B
A * B
A / B
```

Also learned matrix multiplication:

```python
A @ B
```

and:

```python
np.dot(A, B)
```

---

## Matrix Transpose

Practiced:

```python
A.T
```

to obtain the transpose of a matrix.

---

# 🔗 Array Stacking

File: `array_operations.ipynb`

Practiced combining arrays using:

### Vertical Stack

```python
np.vstack((a, b))
```

### Horizontal Stack

```python
np.hstack((a, b))
```

### Column Stack

```python
np.column_stack((a, b))
```

Also practiced stacking 2D arrays.

---

# ✂️ Array Splitting

File: `array_operations.ipynb`

Learned how to split arrays into multiple parts.

### Horizontal Split

```python
np.hsplit(c, 2)

np.hsplit(c, 4)
```

### Vertical Split

```python
np.vsplit(c, 2)

np.vsplit(c, 4)
```

---

# 🧪 Practice and Exercises

File: `exersises.ipynb`

The exercises apply the NumPy concepts learned so far to practical problems.

---

## 1. Valid Sudoku

Created a Sudoku matrix using NumPy and checked whether it is valid.

The solution practices:

* 2D arrays
* Row operations
* Column operations
* Array slicing
* Matrix sections
* `axis`
* `np.sum()`
* Loops
* Conditions
* Functions

The Sudoku validation checks:

```text
Rows
 ↓
Columns
 ↓
3 × 3 Squares
 ↓
Valid / Invalid
```

---

## 2. Student Data Analysis

Created a NumPy matrix containing:

```text
Age
Math Marks
Science Marks
```

Practiced:

* `shape`
* Column selection
* Mean
* Maximum
* Boolean indexing
* Conditional filtering
* Array modification
* Column-wise calculations

Examples of tasks practiced:

```text
Find matrix shape
Find average age
Extract Math marks
Find highest Science mark
Find students scoring > 90 in Math
Increase Math marks by 5
Find students younger than 19
Calculate average marks
Find students scoring at least 80 in both subjects
Replace Science marks below 75 with 0
```

---

# 🧠 Concepts Learned So Far

```text
NumPy
│
├── Array Creation
│
├── Array Generation
│   ├── arange
│   ├── zeros
│   ├── ones
│   └── linspace
│
├── Random Generation
│   ├── rand
│   ├── randn
│   └── randint
│
├── Array Attributes
│   ├── shape
│   ├── size
│   └── dtype
│
├── Array Methods
│   ├── min
│   ├── max
│   ├── sum
│   ├── mean
│   ├── std
│   ├── argmax
│   └── argmin
│
├── Reshaping
│
├── Indexing
│
├── Slicing
│
├── Boolean Indexing
│
├── Arithmetic Operations
│
├── Broadcasting
│
├── Copying
│   ├── Reference
│   └── copy()
│
├── Matrix Operations
│   ├── Addition
│   ├── Subtraction
│   ├── Multiplication
│   ├── Division
│   ├── Matrix Multiplication
│   └── Transpose
│
├── Stacking
│   ├── vstack
│   ├── hstack
│   └── column_stack
│
└── Splitting
    ├── hsplit
    └── vsplit
```

---

# 📓 Notebooks

| Notebook                 | Main Topics                                                               |
| ------------------------ | ------------------------------------------------------------------------- |
| `Arrays.ipynb`           | Array creation, generation, random arrays, attributes, methods, reshaping |
| `array_indexing.ipynb`   | Indexing, slicing, matrix indexing, Boolean indexing                      |
| `array_operations.ipynb` | Arithmetic, broadcasting, copying, matrix operations, stacking, splitting |
| `exersises.ipynb`        | Sudoku validation and student-data problems                               |

---

# 🎯 Current Progress

### Python

* [x] Python Phase 1 completed

### Python Libraries

* [x] NumPy — Currently Learning
* [ ] Pandas
* [ ] Matplotlib
* [ ] Seaborn
* [ ] SciPy

---

# 🚀 Next

After completing NumPy, I will continue with:

```text
NumPy
   ↓
Pandas
   ↓
Matplotlib
   ↓
Seaborn
   ↓
SciPy
```

This will form the foundation for the next stage of my **Data Science journey**.
