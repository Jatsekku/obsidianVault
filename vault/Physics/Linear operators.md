#vectorSpace

$$
\begin{gathered}
M = \begin{bmatrix}
m_{11} && m_{12} && \dots && m_{1j} \\
m_{21} && m_{22} && \dots && m_{2j} \\
\vdots && \vdots && \ddots && \vdots \\
m_{i1} && m_{i2} && \dots && m_{ij} \\
\end{bmatrix} \\\\

m_{ij} \in \mathbb{C}
\end{gathered}
$$

$$
\begin{gathered}
M \ket{A} = \ket{B} \\\\
\begin{bmatrix}
	m_{11} && m_{12} && \dots && m_{1j} \\
	m_{21} && m_{22} && \dots && m_{2j} \\
	\vdots && \vdots && \ddots && \vdots \\
	m_{i1} && m_{i2} && \dots && m_{ij} \\
\end{bmatrix} \begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} = \begin{bmatrix}
	\beta_{1}\\
	\beta_{2} \\
	\vdots \\
	\beta_{i}
\end{bmatrix} \\\\
m_{ij}, \alpha_{i}, \beta_{i} \in \mathbb{C}

\end{gathered}
$$
## Axioms
1. Multiplying input vector has to be translated to the same multiplication of output vector:
$$
\begin{gathered}
M z\ket{A} = z\ket{B} \\\\
\begin{bmatrix}
	m_{11} && m_{12} && \dots && m_{1j} \\
	m_{21} && m_{22} && \dots && m_{2j} \\
	\vdots && \vdots && \ddots && \vdots \\
	m_{i1} && m_{i2} && \dots && m_{ij} \\
\end{bmatrix} \cdot z \cdot \begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} = z \cdot \begin{bmatrix}
	\beta_{1}\\
	\beta_{2} \\
	\vdots \\
	\beta_{i}
\end{bmatrix} \\\\
m_{ij}, z, \alpha_{i}, \beta_{i} \in \mathbb{C}
\end{gathered}
$$
 2. Applying operator on vectors sum is equal to sum of those same vectors treated with operator independently:
$$
\begin{gathered}
M\left(\ket{A} + \ket{B} \right) = M \ket{A} + M\ket{B} \\\\
\begin{bmatrix}
	m_{11} && m_{12} && \dots && m_{1j} \\
	m_{21} && m_{22} && \dots && m_{2j} \\
	\vdots && \vdots && \ddots && \vdots \\
	m_{i1} && m_{i2} && \dots && m_{ij} \\
\end{bmatrix} \left(\begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} + \begin{bmatrix}
	\beta_{1}\\
	\beta_{2} \\
	\vdots \\
	\beta_{i}
\end{bmatrix} \right) = \begin{bmatrix}
	m_{11} && m_{12} && \dots && m_{1j} \\
	m_{21} && m_{22} && \dots && m_{2j} \\
	\vdots && \vdots && \ddots && \vdots \\
	m_{i1} && m_{i2} && \dots && m_{ij} \\
\end{bmatrix} \begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} + \begin{bmatrix}
	m_{11} && m_{12} && \dots && m_{1j} \\
	m_{21} && m_{22} && \dots && m_{2j} \\
	\vdots && \vdots && \ddots && \vdots \\
	m_{i1} && m_{i2} && \dots && m_{ij} \\
\end{bmatrix} \begin{bmatrix}
	\beta_{1}\\
	\beta_{2} \\
	\vdots \\
	\beta_{i}
\end{bmatrix}
\\\\
m_{ij}, \alpha_{i}, \beta_{i} \in \mathbb{C}
\end{gathered}
$$

## Eigenvectors and eigenvalues
$$
\begin{gathered}
M\ket{\lambda} = \lambda \ket{\lambda} \\\\
\text{where:} \\
\ket{\lambda} \text{ - eigenvector} \\
\lambda \text{ - eigenvalue}
\end{gathered}
$$