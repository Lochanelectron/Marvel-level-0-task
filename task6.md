# Task 6: The Matrix Puzzle — Decoding with NumPy

## Objective

The goal of this task was to decode a scrambled numerical matrix and reveal a hidden image using **NumPy** for matrix manipulation and **Matplotlib** for visualization.

I used **Google Colab** so I didn’t need to install any libraries locally.

---

## Tools Used

* Python
* NumPy (array manipulation)
* Matplotlib (data visualization)
* Google Colab (cloud notebook environment)

---

##  1: Upload the Encoded File

The encoded matrix was provided in `.npy` format.

Steps followed:

* I opened Google Colab.
* I created a new notebook.
* I uploaded the file using the **Files panel** on the left sidebar.

To confirm that the file was uploaded correctly, I ran:

```python
import os
os.listdir()
```

This displayed all files in the current working directory and confirmed that the `.npy` file was available.

---

##  2: Import Required Libraries

Next, I imported the libraries required for the task.

```python
import numpy as np
import matplotlib.pyplot as plt
```

* **NumPy** is used for numerical operations and matrix manipulation.
* **Matplotlib** is used to visualize the matrix as an image.

---

##  3: Load the Encoded Array

I loaded the encoded `.npy` file using NumPy.

```python
data = np.load("encoded_array.npy")
```

Then I inspected the structure of the array.

```python
print(data.shape)
print(data.size)
```

This helped me understand the total number of elements stored in the encoded array.

---

##  4: Reshape the Array into a Square Matrix

The encoded data was stored as a **1D array**, but images require a **2D matrix**.

To fix this, I calculated the square root of the total number of elements and reshaped the array.

```python
size = int(np.sqrt(data.size))
matrix = data.reshape(size, size)
```

This converted the flat array into a square matrix representing image pixels.

---

##  5: Visualize the Matrix as an Image

After reshaping the array, I visualized it using Matplotlib.

```python
plt.imshow(matrix, cmap="gray")
plt.axis("off")
plt.show()
```

At first the image appeared **scrambled or incorrectly oriented**, which meant further transformations were needed.

---

##  6: Decode the Image

Based on the clues provided in the task, I experimented with different NumPy transformations such as:

* Transposing the matrix
* Flipping the matrix vertically
* Flipping the matrix horizontally

Example transformation:

```python
matrix = matrix.T
matrix = np.flipud(matrix)
```

After applying the correct combination of transformations, the hidden image became visible.

---

## Outcome

Through this task I learned:

* How to load `.npy` files using NumPy
* How to reshape arrays into matrices
* Basic NumPy operations like transpose and flipping
* How to visualize 2D arrays using Matplotlib

Overall, this task provided a simple introduction to working with **NumPy arrays and data visualization in Python**.

https://github.com/user-attachments/assets/caafce82-ee8f-40d0-a06f-495a1de09feb


