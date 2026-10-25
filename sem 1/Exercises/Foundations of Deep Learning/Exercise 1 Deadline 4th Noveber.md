
4.

Bertrand's Box Paradox is a famous probability problem that demonstrates how conditional probability works and why our intuition about probability can sometimes be incorrect.


## Bertrand's Box Paradox

- **Definition:** A conditional probability problem demonstrating how observing an outcome changes the probability of an underlying event.
- **Cards:** BB (black-black), WW (white-white), BW (black-white).
- **Probability of seeing black:** $P(B)=1/2$.
- **Probability of seeing white:** $P(W)=1/2$.
- **Other side black given visible black:** $P(BB\mid B)=2/3$.
- **Other side black given visible white:** $P(BW\mid W)=1/3$.

**Key concept:** The outcomes must be weighted by how likely they are to produce the observed side. This is an application of Bayes' theorem.

---

## Bertrand's Box Paradox — Probabilities

### Problem Setup

Three cards:
- **BB** — Both sides black
- **WW** — Both sides white
- **BW** — One side black, one side white

### Probability Table

| Event                                    | Probability | Percentage |
| ---------------------------------------- | ----------- | ---------- |
| Card shows black                         | $1/2$       | 50%        |
| Card shows white                         | $1/2$       | 50%        |
| Other side is black, given visible black | $2/3$       | 66.67%     |
| Other side is black, given visible white | $1/3$       | 33.33%     |

### Calculations

**1. Probability of seeing black or white**

$$
P(B)=\frac{2+1}{6}=\boxed{\frac12}
$$

$$
P(W)=\frac{2+1}{6}=\boxed{\frac12}
$$

**2. Probability that the other side is black, given black**

$$
P(BB\mid B)=\frac{2}{3}=\boxed{66.67\%}
$$

**3. Probability that the other side is black, given white**

$$
P(BW\mid W)=\frac{1}{3}=\boxed{33.33\%}
$$

### Key Concept: Conditional Probability

$$
\boxed{P(A\mid B)=\frac{P(A\cap B)}{P(B)}}
$$

Where:
- $P(A\mid B)$ = Probability of A given B
- $P(A\cap B)$ = Probability of both A and B
- $P(B)$ = Probability of B

### Key Takeaway

Bertrand's Box Paradox demonstrates that conditional probability depends on the observed outcome.

- Given **black**: 2 out of 3 possible visible black sides have black on the reverse.
- Given **white**: 1 out of 3 possible visible white sides have black on the reverse.

**Conclusion:** Observing a black side makes the BB card more likely than the BW card.

---

Final answers  

Question Result  
1. P(black up), P(white up) 1/2, 1/2  
2. P(hidden black | visible black) 2/3  
3. P(hidden black | visible white) 1/3

----
### Bertrand's Box Paradox — Bayes' Theorem

$$
P(BB\mid B)=\frac{P(B\mid BB)P(BB)}{P(B)}
$$

**We know:**

$$
P(B\mid BB)=1,\quad P(BB)=\frac13
$$
$$
P(B)=\frac12
$$

**Therefore:**

$$
P(BB\mid B)=\frac{1\times\frac13}{\frac12}
=\boxed{\frac23}
$$

---


# Bertrand's Box Paradox — Solution

## 1. Probability of Observing Black or White

The three cards are:

- **BB:** Both sides black
- **WW:** Both sides white
- **BW:** One side black and one side white

The **BB** card always shows black, the **WW** card always shows white, and the **BW** card shows either color with probability $1/2$.

**Probability of observing black:**

$$
\begin{aligned}
P(\text{black up}) &= P(BB) + P(BW)\cdot P(\text{black up}\mid BW)\\
&= \frac13 + \frac13 \times \frac12\\
&= \boxed{\frac12}
\end{aligned}
$$

**Probability of observing white:**

$$
\begin{aligned}
P(\text{white up}) &= P(WW) + P(BW)\cdot P(\text{white up}\mid BW)\\
&= \frac13 + \frac13 \times \frac12\\
&= \boxed{\frac12}
\end{aligned}
$$

---

## 2. Probability the Hidden Side Is Black, Given Black Is Visible

If black is visible, the card must be either **BB** or **BW**.

Among the three equally likely black-facing sides:
- Two black sides belong to **BB**.
- One black side belongs to **BW**.

Therefore, two out of three possibilities have a black hidden side.

**Using Bayes' Theorem:**

$$
P(A\mid B)=\frac{P(B\mid A)P(A)}{P(B)}
$$

**Calculation:**

$$
\begin{aligned}
P(\text{hidden black}\mid\text{visible black})
&= P(BB\mid\text{visible black})\\
&= \frac{P(\text{visible black}\mid BB)\cdot P(BB)}
{P(\text{visible black})}\\
&= \frac{1\times\frac13}{\frac12}\\
&= \boxed{\frac23}
\end{aligned}
$$

**Answer:** $66.67\%$

---

## 3. Probability the Hidden Side Is Black, Given White Is Visible

If white is visible, the card must be either **WW** or **BW**.

Among the three equally likely white-facing sides:
- Two white sides belong to **WW**.
- One white side belongs to **BW**.

Only the **BW** card has black on the reverse.

**Using Bayes' Theorem:**

$$
\begin{aligned}
P(\text{hidden black}\mid\text{visible white})
&= P(BW\mid\text{visible white})\\
&= \frac{P(\text{visible white}\mid BW)\cdot P(BW)}
{P(\text{visible white})}\\
&= \frac{\frac12\times\frac13}{\frac12}\\
&= \boxed{\frac13}
\end{aligned}
$$

**Answer:** $33.33\%$

---

## Final Answers

| Question | Probability | Percentage |
|---|---|---|
| Black side visible | $\frac12$ | 50% |
| White side visible | $\frac12$ | 50% |
| Hidden black given visible black | $\frac23$ | 66.67% |
| Hidden black given visible white | $\frac13$ | 33.33% |

### Key Concept

**Conditional Probability and Bayes' Theorem**

$$
\boxed{P(A\mid B)=\frac{P(A\cap B)}{P(B)}}
$$

$$
\boxed{P(A\mid B)=\frac{P(B\mid A)P(A)}{P(B)}}
$$

**Key Takeaway:** Observing a particular color changes the probabilities of which card was selected. This is an application of conditional probability and Bayes' theorem.

---



## Law of Total Probability

**Definition:** The Law of Total Probability calculates the overall probability of an event by considering all possible mutually exclusive cases.

### General Formula

$$
\boxed{P(A)=\sum_{i=1}^{n}P(A\mid B_i)P(B_i)}
$$

Where:
- $P(A)$ = Total probability of event A
- $P(A\mid B_i)$ = Probability of A given event $B_i$
- $P(B_i)$ = Probability of event $B_i$
- $B_1,B_2,\ldots,B_n$ = Mutually exclusive and exhaustive events

### Example: Bertrand's Box Paradox

Three cards:
- **BB:** Black–Black
- **WW:** White–White
- **BW:** Black–White

**Question:** What is the probability of observing a black side?

Using the Law of Total Probability:

$$
\begin{aligned}
P(\text{black up}) ={}&
P(B\mid BB)P(BB)\\
&+P(B\mid WW)P(WW)\\
&+P(B\mid BW)P(BW)
\end{aligned}
$$

We know:

$$
P(B\mid BB)=1
$$

$$
P(B\mid WW)=0
$$

$$
P(B\mid BW)=\frac12
$$

Each card has a probability of $\frac13$ of being selected.

**Calculation:**

$$
\begin{aligned}
P(\text{black up})
&=1\times\frac13+0\times\frac13+\frac12\times\frac13\\
&=\frac13+\frac16\\
&=\boxed{\frac12=50\%}
\end{aligned}
$$

### Law of Total Probability vs. Bayes' Theorem

| Concept | Purpose |
|---|---|
| Law of Total Probability | Calculates the overall probability of an event |
| Bayes' Theorem | Calculates the probability of a hypothesis given observed evidence |

**Law of Total Probability:**

$$
\boxed{P(A)=\sum_{i=1}^{n}P(A\mid B_i)P(B_i)}
$$

**Bayes' Theorem:**

$$
\boxed{P(A\mid B)=\frac{P(B\mid A)P(A)}{P(B)}}
$$

### Key Takeaway

The **Law of Total Probability** combines the probabilities of all possible cases to calculate the overall probability of an event.

---


5.

"""Simple example file."""


def example_function(input_variable: float) -> float:
    """Multiply an input variable by two.

    Args:
        input_variable: Input for calculation.

    Returns:
        The input times two.
    """
    # START TODO #################
    return input_variable * 2
    # END TODO ###################


conda activate
python example_script.py
python -m tests.test_example


---

6.

```
import numpy as np


def main():
    # create input matrices
    A = np.array(np.arange(4))
    B = np.array([-1, 3])
    print("\n---------- Input matrices shape, type and content:")
    print(f"A (shape: {A.shape}, type: {type(A)}) = {A}")
    print(f"B (shape: {B.shape}, type: {type(B)}) = {B}")
    print("\n---------- Matrix multiplication on those matrices does not work:")
    
    try:
        np.matmul(A, B)
    except ValueError as e:
        print(f"Error type: {type(e)} message: {e}")
        
    print("\n---------- Reshape A from shape (4,) to shape (2,2) and store it in C:")
    C = A.reshape([2, 2])
    print(f"C shape: {C.shape}, content:\n{C}")
    print("\n---------- Now matrix multiplication of C (2,2) with B (2,) works:")
    matmul_result = np.matmul(C, B)
    print(f"Matrix multiplication result:\n{matmul_result}")
    print("\n---------- When adding C (2,2) and B (2,), B will be automatically "
          "broadcasted to match the shape of C.")
    add_result = np.add(C, B)
    print(f"Addition result:\n{add_result}")
    print("\n---------- The star operator (*) will do an element-wise multiplication between C (2,2) and B (2,). "
          "Again, B will be broadcasted to fit the shape of C. ")
    print(f"Element-wise multiplication result:\n{C * B}")
    print("\n---------- np.diag can transform the vector B (2,) into a diagonal matrix of shape (2,2)")
    print(f"B as diagonal matrix:\n{np.diag(B)}")
    print("\n---------- Use np.transpose to transpose the matrix C")
    print(f"Transpose result:\n{np.transpose(C)}")


if __name__ == '__main__':
    main()
```

---


Todo: Run the script run_numpy_arrays.py. We will walk you through its code and output during this exercise.
Todo: In file lib/eigendecomp.py, complete the function get_matrix_from_eigdec to return the square symmetric matrix A, given its eigenvalues λ1, . . . , λn and eigenvectors Q as an input. Note: We are using type hints to make the code more readable and give you hints about the input and output
Todo: Complete the get_euclidean_norm function without using numpy.linalg.norm to show that you know how to avoid using a manual loop in favor of a vectorized numpy expression.
Todo: Complete the get_dot_product function
Todo: Complete the get_inverse function by using the assumption that A is symmetric, therefore A−1 = QΛ −1QT with Λ −1 = diag(λ −1 1 , . . . , λ−1 n ) is the inverse of A. Do not use numpy.linalg.inv. You can invert the diagonal matrix Λ without it.
Todo: Complete std_normal and normal in lib/distributions.py, then run plot_normal.py

Run python -m tests.test_distributions to test your implementation


# NumPy Tensors & Eigendecomposition

## 1. NumPy Tensors

**Definition:** NumPy tensors are multidimensional arrays used to store and manipulate numerical data efficiently.

The fundamental NumPy object is `ndarray`.

### Creating Arrays

```python
import numpy as np

A = np.array(np.arange(4))
B = np.array([-1, 3])

print(A.shape, A)
print(B.shape, B)
```

**Output:**

```text
(4,) [0 1 2 3]
(2,) [-1  3]
```

- `shape` describes the dimensions of an array.
- `ndarray` is NumPy's multidimensional array class.
- `(4,)` represents a one-dimensional array with 4 elements.

### Reshaping Arrays

```python
C = A.reshape(2, 2)
print(C)
```

**Output:**

```text
[[0 1]
 [2 3]]
```

**Shape:** $(2,2)$

### Matrix Multiplication

Matrix multiplication requires compatible dimensions.

$$
A_{m\times n}B_{n\times p}=C_{m\times p}
$$

```python
result = np.matmul(C, B)
# Equivalent:
result = C @ B
print(result)
```

**Output:**

```text
[3 7]
```

**Calculation:**

$$
\begin{bmatrix}
0&1\\
2&3
\end{bmatrix}
\begin{bmatrix}
-1\\
3
\end{bmatrix}
=
\begin{bmatrix}
3\\
7
\end{bmatrix}
$$

### Broadcasting

**Definition:** Broadcasting allows NumPy to perform operations on arrays with different but compatible shapes.

```python
print(np.add(C, B))
```

**Output:**

```text
[[-1  4]
 [ 1  6]]
```

Here, `B` is broadcast across both rows of `C`.

### Element-wise Multiplication

The `*` operator multiplies corresponding elements.

```python
print(C * B)
```

**Output:**

```text
[[ 0  3]
 [-2  9]]
```

**Difference:**

- `@` or `np.matmul()` — Matrix multiplication
- `*` — Element-wise multiplication
- `np.add()` — Element-wise addition

### Diagonal Matrix

```python
print(np.diag(B))
```

**Output:**

```text
[[-1  0]
 [ 0  3]]
```

### Matrix Transpose

**Definition:** Transposing a matrix exchanges its rows and columns.

$$
(A^T)_{ij}=A_{ji}
$$

```python
print(C.T)
# Equivalent:
print(np.transpose(C))
```

**Output:**

```text
[[0 2]
 [1 3]]
```

---

## 2. Vectorization in NumPy

**Definition:** Vectorization performs operations on entire arrays without manually iterating through individual elements.

### Using Loops (Slower)

```python
numbers = np.random.random(1000000)

total = 0
for number in numbers:
    total += number ** 2
```

### Using Vectorization (Faster)

```python
numbers = np.random.random(1000000)

total = (numbers ** 2).sum()
```

**Mathematical Operation:**

$$
\sum_{i=1}^{n}x_i^2
$$

**Key Point:** Vectorized NumPy operations are generally faster because they execute optimized compiled code internally.

---

## 3. Eigendecomposition

**Definition:** Eigendecomposition represents a square matrix using its eigenvalues and eigenvectors.

For a real symmetric matrix:

$$
\boxed{A=Q\Lambda Q^T}
$$

Where:

- $A$ = Original square symmetric matrix
- $Q$ = Matrix containing eigenvectors as columns
- $\Lambda$ = Diagonal matrix containing eigenvalues
- $Q^T$ = Transpose of the eigenvector matrix

### Eigenvalues and Eigenvectors

An eigenvector satisfies:

$$
\boxed{Av=\lambda v}
$$

Where:
- $A$ = Square matrix
- $v$ = Eigenvector
- $\lambda$ = Eigenvalue

**Meaning:** Multiplying an eigenvector by matrix $A$ changes its magnitude (and possibly direction), but keeps it along the same line.

### Example Matrix

$$
A=
\begin{bmatrix}
7&-\sqrt3\\
-\sqrt3&5
\end{bmatrix}
$$

Using NumPy:

```python
import numpy as np

A = np.array([
    [7, -np.sqrt(3)],
    [-np.sqrt(3), 5]
])

eigenvalues, Q = np.linalg.eigh(A)
```

For symmetric matrices, `np.linalg.eigh()` is preferred.

---

## 4. Reconstructing a Matrix from Eigendecomposition

**Formula:**

$$
\boxed{A=Q\Lambda Q^T}
$$

**NumPy Implementation:**

```python
diagonal_matrix = np.diag(eigenvalues)

A = Q @ diagonal_matrix @ Q.T
```

- `np.diag()` constructs the diagonal eigenvalue matrix.
- `Q.T` computes the transpose.
- `@` performs matrix multiplication.

---

## 5. Euclidean Norm

**Definition:** The Euclidean norm calculates the length or magnitude of a vector.

**Formula:**

$$
\boxed{\|x\|_2=\sqrt{\sum_{i=1}^{n}x_i^2}}
$$

### Example

$$
x=
\begin{bmatrix}
3\\
4
\end{bmatrix}
$$

$$
\|x\|_2=\sqrt{3^2+4^2}
$$

$$
=\sqrt{25}=\boxed{5}
$$

### NumPy Implementation

```python
def get_euclidean_norm(vector):
    return np.sqrt(np.sum(vector ** 2))
```

**Important:** Avoid manual loops and `np.linalg.norm()` for this assignment.

---

## 6. Dot Product

**Definition:** The dot product multiplies corresponding elements of two vectors and sums the results.

**Formula:**

$$
\boxed{a\cdot b=\sum_{i=1}^{n}a_i b_i}
$$

### Example

$$
a=[1,2],\quad b=[3,4]
$$

$$
a\cdot b=(1\times3)+(2\times4)
$$

$$
=\boxed{11}
$$

### NumPy Implementation

```python
def get_dot_product(vector1, vector2):
    return np.sum(vector1 * vector2)
```

Alternative:

```python
np.dot(vector1, vector2)
```

### Orthogonality

Two vectors are orthogonal when:

$$
\boxed{a\cdot b=0}
$$

**Orthonormal vectors** satisfy:

1. Each vector has unit length:

$$
\|q_i\|_2=1
$$

2. Different vectors are orthogonal:

$$
q_i^Tq_j=0,\quad i\neq j
$$

Together:

$$
\boxed{Q^TQ=I}
$$

---

## 7. Matrix Inverse Using Eigendecomposition

For a symmetric, invertible matrix:

$$
\boxed{A^{-1}=Q\Lambda^{-1}Q^T}
$$

Where:

$$
\Lambda^{-1}=
\operatorname{diag}
\left(
\frac1{\lambda_1},
\frac1{\lambda_2},
\ldots,
\frac1{\lambda_n}
\right)
$$

### NumPy Implementation

```python
inverse_diagonal = np.diag(1.0 / eigenvalues)

A_inverse = Q @ inverse_diagonal @ Q.T
```

**Important:**
- Do not use `np.linalg.inv()` for this assignment.
- The inverse exists only when all eigenvalues are nonzero.

### Inverse Property

$$
\boxed{AA^{-1}=I}
$$

Where $I$ is the identity matrix.

---

## 8. Summary

| Concept | Formula / NumPy |
|---|---|
| Matrix multiplication | `A @ B` |
| Element-wise multiplication | `A * B` |
| Addition | `np.add(A, B)` |
| Reshape | `A.reshape(2, 2)` |
| Transpose | `A.T` |
| Diagonal matrix | `np.diag(x)` |
| Eigendecomposition | $A=Q\Lambda Q^T$ |
| Eigenvector equation | $Av=\lambda v$ |
| Euclidean norm | $\sqrt{\sum x_i^2}$ |
| Dot product | $\sum a_i b_i$ |
| Orthogonality | $a\cdot b=0$ |
| Orthonormality | $Q^TQ=I$ |
| Matrix inverse | $A^{-1}=Q\Lambda^{-1}Q^T$ |

### Key Takeaways

- **NumPy arrays** are fundamental for numerical computation and deep learning.
- **Broadcasting** enables operations between compatible arrays of different shapes.
- **Vectorization** avoids slow Python loops.
- **Eigendecomposition** represents matrices using eigenvalues and eigenvectors.
- **Euclidean norm** measures vector length.
- **Dot product** measures algebraic alignment between vectors.
- **Orthonormal eigenvectors** have unit length and are mutually perpendicular.
- **Matrix inversion** can be performed using eigendecomposition when the matrix is symmetric and invertible.

---