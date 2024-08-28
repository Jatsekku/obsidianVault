# Inverse Matrices

$$AA^{-1} = A^{-1}A = I_{n}$$
- matrix is invertible only when [[#determinant]] is not equal to 0: $$det(A) \neq 0$$
# Determinant

For 2x2 matrix A determinant is defined as follows: \
$$det(A) = |A| = A_{0,0} \cdot A_{1,1} - A_{0,1} \cdot A_{1,0}$$
# Transpose

$$ A^{T} = A_{i,j}^T = A_{j,i} $$
for example: 
$$
\begin{bmatrix}
1 && 2 \\
3 && 4 \\
5 && 6 \\
\end{bmatrix}^{T}
=
\begin{bmatrix}
1 && 3 && 5 \\
2 && 4 && 6 \\
\end{bmatrix}
$$
# Conjugate
- This operation makes sense only for complex-valued matrices.
$$
A = 
\begin{bmatrix}
x_{0,0} && x_{0,1} && \dots && x_{0,m-1} \\
x_{1,0} && x_{1,1} && \dots && x_{1,m-1} \\
\vdots && \vdots && \ddots && \vdots \\
x_{n-1,0} && x_{n-1,1} && \dots && x_{n-1,m-1} \\

\end{bmatrix}
$$
$$
\overline A = 
\begin{bmatrix}
\overline x_{0,0} && \overline x_{0,1} && \dots && \overline x_{0,m-1} \\
\overline x_{1,0} && \overline x_{1,1} && \dots && \overline x_{1,m-1} \\
\vdots && \vdots && \ddots && \vdots \\
\overline x_{n-1,0} && \overline x_{n-1,1} && \dots && \overline x_{n-1,m-1} \\

\end{bmatrix}
$$

# Adjoint
- Combination of [[#Conjugate]] and [[#Transpose]]
$$ A^{\dagger} = \overline{(A^{T})} = (\overline{A})^{T}$$

# Unitary matrix
- A matrix is unitary when it's inverse is equal to its [[#Adjoint]] :
  $$ U^{-1} = U^{\dagger}$$ so the following criteria has to be met:
  $$ U^{\dagger}U = UU^{\dagger} = I_{n}$$

  # Inner product
  - Applied only for vectors