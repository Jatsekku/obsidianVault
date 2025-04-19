1. Observable is represented by [[Hermitian operators]]
2. Possible measurement outcomes are defined by [[Linear operators#Eigenvectors and eigenvalues|eigenvalues]]
3. Differentiable states are represented by orthogonal vectors.
4. If [[Vector space#Kets|ket]] $\ket{A}$ is vector state of measured system and we measure observable $L$ then the observed probability is equal to:
$$
\begin{gathered}
P(\lambda_{i}) = \braket{A|\lambda_{i}} \braket{\lambda_{i}|A} = {|\braket{A|\lambda_{i}}|^{2}}\\\\
\text{where:} \\
\lambda_{i} \text{ - eigenvalue of Hermitian operator }L \\
\ket{\lambda_{i}}, \bra{\lambda_{i}} \text{ - eigenvectors of Hermitian operator }L \\

\end{gathered}
$$
## Examples

### Spin operators
Let's denote two orthogonal state vectors as follows:
$$
\begin{gathered}
\ket{g} = \begin{bmatrix}
1 \\
0
\end{bmatrix}, \ket{d} = \begin{bmatrix}
0 \\
1
\end{bmatrix} 
\end{gathered}
$$
Let's denote spin operator along z-axis as $\sigma_{z}$. 
We would like to know it's form if $\ket{g}$ and $\ket{d}$ are it's eigenvectors and it's eigenvalues are $\pm 1$.
We can express it as follows:

$$
\sigma_{z}\ket{g} = \ket{g} \tag{1} \label{eq1}
$$
$$
\sigma_{z}\ket{d} = -\ket{d} \tag{2} \label{eq2}
$$
Let's express it in matrix form:

$$
\begin{bmatrix}
{(\sigma_{z}})_{11} & {(\sigma_{z}})_{12} \\
{(\sigma_{z}})_{21} & {(\sigma_{z}})_{21} \\
\end{bmatrix} \begin{bmatrix}
1 \\
0
\end{bmatrix} = \begin{bmatrix}
1 \\
0
\end{bmatrix}
\tag{3}
\label{eq3}
$$

$$
\begin{bmatrix}
{(\sigma_{z}})_{11} & {(\sigma_{z}})_{12} \\
{(\sigma_{z}})_{21} & {(\sigma_{z}})_{21} \\
\end{bmatrix} \begin{bmatrix}
1 \\
0
\end{bmatrix} = -\begin{bmatrix}
0 \\
1
\end{bmatrix}
\tag{4}
\label{eq4}
$$

We can solve it to get matrix elements values of $\sigma_{z}$:

From $\refeq{eq3}$ :  
$$
\begin{gathered}
(\sigma_{z})_{11} \cdot 1 + (\sigma_{z})_{12} \cdot 0 = 1 \rightarrow  (\sigma_{z})_{11} = 1 \\
(\sigma_{z})_{21} \cdot 1 + (\sigma_{z})_{22} \cdot 0 = 0 \rightarrow  (\sigma_{z})_{21} = 0 \\
\end{gathered}
$$
From $\refeq{eq4}$ :
$$
\begin{gathered}
(\sigma_{z})_{11} \cdot 0 + (\sigma_{z})_{12} \cdot 1 = 0 \rightarrow  (\sigma_{z})_{12} = 0 \\
(\sigma_{z})_{11} \cdot 0 + (\sigma_{z})_{12} \cdot 1 = -1 \rightarrow  (\sigma_{z})_{22} = -1 \\
\end{gathered}
$$
Which gives us one and only solution of $\sigma_{z}$:
$$
\sigma_{z} = \begin{bmatrix}
1 & 0 \\
0 & -1 \\
\end{bmatrix}
$$

We can apply the same procedure for $\sigma_{x}$ and $\sigma_{x}$. Let's start by recalling that 

TO DO

Which in effect, gives us three Pauli Matrix:
$$
\begin{gathered}
\sigma_{z} = \begin{bmatrix}
1 & 0 \\
0 & -1 \\
\end{bmatrix} \\\\
\sigma_{x} = \begin{bmatrix}
0 & 1 \\
1 & 0 \\
\end{bmatrix}\\\\
\sigma_{y} = \begin{bmatrix}
0 & -i \\
i & 0 \\
\end{bmatrix}
\end{gathered}
$$
 RECALL HOW TO FIND EIGEN VALUES AND EIGENVECTORS
 