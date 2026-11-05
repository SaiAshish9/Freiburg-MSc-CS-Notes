
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


5. ![[Pasted image 20261027193919.png]]

- **Todo:** In file `lib/eigendecomp.py`, complete the function `get_matrix_from_eigdec` to return the square symmetric matrix $A$, given its eigenvalues $\lambda_1, \ldots, \lambda_n$ and eigenvectors $Q$ as an input. **Note:** We are using type hints to make the code more readable and give you hints about the input and output.
- Run `python -m tests.test_matrix_from_eigdec` to test your implementation.

- **Todo:** Complete the `get_euclidean_norm` function without using `numpy.linalg.norm` to show that you know how to avoid using a manual loop in favor of a vectorized numpy expression.
- Run `python -m tests.test_euclidean_norm` to test your implementation.

- **Todo:** Complete the `get_dot_product` function.
- The two functions mentioned above take vectors as input and are used to show that the columns of $Q$ are orthonormal, i.e. the columns are of unit length and are pairwise orthogonal (their dot product is 0).
- Run `python -m tests.test_dot_product` to test your implementation.

- **Todo:** Complete the `get_inverse` function by using the assumption that $A$ is symmetric, therefore $A^{-1} = Q\Lambda^{-1}Q^T$ with $\Lambda^{-1} = \text{diag}(\lambda_1^{-1}, \ldots, \lambda_n^{-1})$ is the inverse of $A$. Do **not** use `numpy.linalg.inv`. You can invert the diagonal matrix $\Lambda$ without it.
- Run `python -m tests.test_inverse` to test your implementation.

---
