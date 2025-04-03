#diracNotion
#vectorSpace
#quantumMechanics

# Dirac notion

## Kets
$$
\begin{gathered}
\ket{A} = \begin{bmatrix}
		\alpha_{1}\\
		\alpha_{2} \\
		\vdots \\
		\alpha_{i}
	\end{bmatrix}\\\\
	\alpha_{i} \in \mathbb{C} 
\end{gathered}
$$
## Ket axioms

1. Sum of two kets is ket: 
$$
\begin{gathered}
\ket{A} + \ket{B} = \ket{C} \\\\
\begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} + \begin{bmatrix}
	\beta_{1}\\
	\beta_{2} \\
	\vdots \\
	\beta_{i}
\end{bmatrix} = \begin{bmatrix}
	\alpha_{1} + \beta_{1}\\
	\alpha_{2} + \beta_{2}\\
	\vdots \\
	\alpha_{i} + \beta_{i}\\
\end{bmatrix} \\\\
\alpha_{i}, \beta_{i} \in \mathbb{C}
\end{gathered}
$$

2. Kets addition is commutative: 
$$
\begin{gathered}
\ket{A} + \ket{B} = \ket{B} + \ket{A} \\\\
\begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} + \begin{bmatrix}
	\beta_{1}\\
	\beta_{2} \\
	\vdots \\
	\beta_{i}
\end{bmatrix} = \begin{bmatrix}
	\beta_{1}\\
	\beta_{2} \\
	\vdots \\
	\beta_{i}
\end{bmatrix} + \begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} \\\\
\alpha_{i}, \beta_{i} \in \mathbb{C}
\end{gathered}
$$
3. Kets addition is associative: 
$$
\begin{gathered}

(\ket{A} + \ket{B}) + \ket{C} = \ket{A} + (\ket{B} + \ket{C}) \\\\
\left( \begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} + \begin{bmatrix}
	\beta_{1}\\
	\beta_{2} \\
	\vdots \\
	\beta_{i}
\end{bmatrix} \right) + \begin{bmatrix}
	\gamma_{1}\\
	\gamma_{2} \\
	\vdots \\
	\gamma_{i}
\end{bmatrix} = \begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} + \left( \begin{bmatrix}
	\beta_{1}\\
	\beta_{2} \\
	\vdots \\
	\beta_{i}
\end{bmatrix} + \begin{bmatrix}
	\gamma_{1}\\
	\gamma_{2} \\
	\vdots \\
	\gamma_{i}
\end{bmatrix} \right) \\\\
\alpha_{i}, \beta_{i} \in \mathbb{C}

\end{gathered}
$$
4. There is one additive identity element: 
$$
\begin{gathered}
\ket{A} + 0 = \ket{A} \\\\
\begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} + \begin{bmatrix}
	0\\
	0 \\
	\vdots \\
	0
\end{bmatrix} = \begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} \\\\
\alpha_{i} \in \mathbb{C}
\end{gathered}
$$
5. For every ket, there is additive inverse element: 
$$
\begin{gathered}
\ket{A} + (-\ket{A}) = 0 \\\\
\begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} + \begin{bmatrix}
	-\alpha_{1}\\
	-\alpha_{2} \\
	\vdots \\
	-\alpha_{i}
\end{bmatrix} = \begin{bmatrix}
	0\\
	0 \\
	\vdots \\
	0
\end{bmatrix} \\\\
\alpha_{i} \in \mathbb{C}
\end{gathered}
$$
6. We can multiply any ket by a complex number:
$$
\begin{gathered}
\ket{zA} = z\ket{A} = \ket{B} \\\\
\begin{bmatrix}
	z\alpha_{1}\\
	z\alpha_{2} \\
	\vdots \\
	z\alpha_{i}
\end{bmatrix} = z\begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} = \begin{bmatrix}
	\beta_{1}\\
	\beta_{2} \\
	\vdots \\
	\beta_{3}
\end{bmatrix} \\\\
z, \alpha_{i}, \beta_{i} \in \mathbb{C}
\end{gathered}
$$
7. ...:  
$$
\begin{gathered}
z(\ket{A} + \ket{B}) = z\ket{A} + z\ket{B} \\\\
z \left(\begin{bmatrix}
		\alpha_{1} \\
		\alpha_{2} \\
		\vdots \\
		\alpha_{i} \\
	\end{bmatrix} + \begin{bmatrix}
		\beta_{1} \\
		\beta_{2} \\
		\vdots \\
		\beta_{i} \\
	\end{bmatrix}
\right) = z\begin{bmatrix}
	\alpha_{1} \\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i} \\
\end{bmatrix} + z\begin{bmatrix}
	\beta_{1} \\
	\beta_{2} \\
	\vdots \\
	\beta_{i} \\
\end{bmatrix}\\\\\\\\

(z+w)\ket{A} = z\ket{A} + w\ket{A} \\\\
(z +w) \begin{bmatrix}
		\alpha_{1} \\
		\alpha_{2} \\
		\vdots \\
		\alpha_{i} \\
	\end{bmatrix}
 = z\begin{bmatrix}
	\alpha_{1} \\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i} \\
\end{bmatrix} + w\begin{bmatrix}
	\alpha_{1} \\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i} \\
\end{bmatrix}\\\\
z,w,\alpha_{i},\beta_{i} \in \mathbb{C}
\end{gathered}
$$

## Bras
$$
\begin{gathered}
\bra{A} = \begin{bmatrix}
		{\alpha_{1}}^{*}, 
		{\alpha_{2}}^{*},
		\cdots,
		{\alpha_{i}}^{*}
	\end{bmatrix}\\\\
	\alpha_{i} \in \mathbb{C}
\end{gathered}
$$

## Bras and kets together

### Inner product of bra and ket

$$
\begin{gathered}
\braket{B|A} \in \mathbb{C} \\\\

\begin{bmatrix}
	{\beta_{1}}^{*},
	{\beta_{2}}^{*},
	\cdots,
	{\beta_{i}}^{*}
\end{bmatrix} \begin{bmatrix}
	\alpha_{1}\\
	\alpha_{2} \\
	\vdots \\
	\alpha_{i}
\end{bmatrix} = ({\beta_{1}}^{*}\alpha_{1} + {\beta_{2}}^{*}\alpha_{2} + \cdots + {\beta_{3}}^{*}\alpha_{3}) \in \mathbb{C}

\end{gathered}
$$
#### Axioms of inner product:
$$
\bra{C}\left( \ket{A} + \ket{B}\right) = \braket{C|A} + \braket{C|B}
$$

$$
\braket{B|A} = {\braket{A|B}}^{*}
$$

