Hermitian operators are special type of [[Linear operators]]

## Conjugate transpose (Hermitian conjugate)
We can apply conjugate to any linear operator. This operation is defined as follows:
$$
\begin{gathered}
M^{\dagger} = \left[ M^{T}\right]^{*} \\\\
\begin{bmatrix}
	m_{11} && m_{12} && \dots && m_{1j} \\
	m_{21} && m_{22} && \dots && m_{2j} \\
	\vdots && \vdots && \ddots && \vdots \\
	m_{i1} && m_{i2} && \dots && m_{ij} \\
\end{bmatrix}^{\dagger} = \begin{bmatrix}
	{m_{11}}^{*} && {m_{21}}^{*} && \dots && {m_{j1}}^{*} \\
	{m_{12}}^{*} && {m_{22}}^{*} && \dots && {m_{j2}}^{*} \\
	\vdots && \vdots && \ddots && \vdots \\
	{m_{1i}}^{*} && {m_{2i}}^{*} && \dots && {m_{ji}}^{*} \\
\end{bmatrix} \\\\
m_{ij} \in \mathbb{C}
\end{gathered}
$$
## Axiom
Hermitian operator is linear operator that has to fulfill following condition:
$$
\begin{gathered}
M = M^{\dagger} \\\\
\begin{bmatrix}
	m_{11} && m_{12} && \dots && m_{1j} \\
	m_{21} && m_{22} && \dots && m_{2j} \\
	\vdots && \vdots && \ddots && \vdots \\
	m_{i1} && m_{i2} && \dots && m_{ij} \\
\end{bmatrix} = \begin{bmatrix}
	{m_{11}}^{*} && {m_{21}}^{*} && \dots && {m_{j1}}^{*} \\
	{m_{12}}^{*} && {m_{22}}^{*} && \dots && {m_{j2}}^{*} \\
	\vdots && \vdots && \ddots && \vdots \\
	{m_{1i}}^{*} && {m_{2i}}^{*} && \dots && {m_{ji}}^{*} \\
\end{bmatrix}\\\\
m_{ij} = {m_{ji}}^{*} \\\\
m_{ij} \in \mathbb{C}
\end{gathered}
$$

From now I'm gonna use $L$ symbol to denote Hermitian operator.

## Important properties
1. All Hermitian operators have real eigenvalues
   Proof: 
$$
L\ket{\lambda} = \lambda \ket{\lambda} \tag{1} \label{eq1}
$$
From definition of Hermitian conjugate, we get:
$$
\bra{\lambda}L^{\dagger} = \bra{\lambda} {\lambda}^{*} \tag{2} \label{eq2}
$$
As $L$ is Hermitian operator, so $L=L^{\dagger}$, we can rewrite $\eqref{eq2}$ as:
$$
\bra{\lambda}L = \bra{\lambda} {\lambda}^{*} \tag{3} \label{eq3}
$$
Next, let's multiply $\eqref{eq1}$ by $\bra{\lambda}$ and $\eqref{eq3}$ by $\ket{\lambda}$ and we get:
$$
\bra{\lambda}L\ket{\lambda} = \lambda \braket{\lambda|\lambda} \tag{4} \label{eq4}
$$
$$
\bra{\lambda}L\ket{\lambda} = {\lambda}^{*}\braket{\lambda|\lambda} \tag{5} \label{eq5}
$$
Finally, we see that $\lambda = {\lambda}^{*}$  (any eigenvalue $(\lambda)$ of any Hermitian operator $(L)$) has to be real.

**Remark :**
I haven't noticed that immediately, but that's indeed obvious when complex conjugate definition will be recalled:
$$
\begin{gathered}
\lambda = \lambda^{*} \\ 
\lambda_{1} + i\lambda_{2} = \lambda_{1} - i\lambda_{2} \\\\\
\lambda_{1} + i\lambda_{2} - \lambda_{1} + i\lambda_{2} = 0 \\
2i\lambda_{2} = 0 \rightarrow \lambda_{2} = 0
\end{gathered}
$$


2. Eigenvectors of Hermitian operator create orthogonal base.
   Proof:

Let's express two eigenvectors ($\lambda_{1}, \lambda_{2}$) of Hermitian operator $L$
$$
L\ket{\lambda_{1}} = \lambda_{1}\ket{\lambda_{1}} \tag{1} \label{eq6}
$$
$$
L\ket{\lambda_{2}} = \lambda_{2}\ket{\lambda_{2}} \tag{2} \label{eq7}
$$
Using the fact that $L$ is Hermitian operator, we can rewrite $\eqref{eq6}$ as:
$$
\bra{\lambda_{1}}L = \lambda_{1}\bra{\lambda_1} \tag{3} \label{eq8}
$$
Next, we can calculate inner product of $\refeq{eq8}$ with $\ket{\lambda_{2}}$ and inner product of $\refeq{eq7}$ with $\bra{\lambda_{1}}$
$$
\bra{\lambda_{1}}L\ket{\lambda_{2}} = \lambda_{1} \braket{\lambda_{1}|\lambda_{2}} \tag{4} \label{eq9}
$$
$$
\bra{\lambda_{1}}L\ket{\lambda_{2}} = \lambda_{2}\braket{\lambda_{1}|\lambda_{2}} \tag{5} \label{eq10}
$$
Finally, let's calc the difference of equations $\refeq{eq9}, \refeq{eq10}$:
$$
\begin{gathered}
\lambda_{1} \braket{\lambda_{1}|\lambda_{2}} = \lambda_{2}\braket{\lambda_{1}|\lambda_{2}} \\\\
\lambda_{1} \braket{\lambda_{1}|\lambda_{2}} - \lambda_{2}\braket{\lambda_{1}|\lambda_{2}} = 0 \\
(\lambda_{1} - \lambda_{2})\braket{\lambda_{1}|\lambda_{2}} = 0
\end{gathered}
$$
We can observe that if eigenvalues $\lambda_{1} \neq \lambda_{1}$ then eigenvectors ($\bra{\lambda_{1}}, \ket{\lambda_2}$) has to be orthogonal (because inner product of two orthogonal vectors is equal 0)
