# Matrix representation

- any quantum gate is represented by [[Matrices#Unitary matrix]] 2x2 matrix.
$$
A = 
\begin{bmatrix}
\epsilon & \zeta \\
\eta & \mu
\end{bmatrix}
$$
- quantum state can be multiplied by matrix gate (which is equivalent to applying gate's operation on this state):
$$

A\ket{\Psi} = 
\begin{bmatrix}
\epsilon & \zeta \\
\eta & \mu
\end{bmatrix}
\begin{bmatrix}
\alpha \\
\beta
\end{bmatrix}
=
\begin{bmatrix}
\epsilon \cdot \alpha + \zeta \cdot \beta\\
\eta \cdot \alpha + \mu \cdot \beta
\end{bmatrix}
= \left(\epsilon \cdot \alpha + \zeta \cdot \beta \right) \cdot \ket{0} 
+ \left( \eta \cdot \alpha + \mu \cdot \beta \right) \cdot \ket{1}

$$

for example X gate is defined as follows:

$$
X =
\begin{bmatrix}
0 & 1 \\
1 & 0 \\
\end{bmatrix}
$$
Let's apply it to basis states:
$$
\begin{gather*}
X\ket{0} = 
\begin{bmatrix}
0 & 1 \\
1 & 0 \\
\end{bmatrix}
\begin{bmatrix}
1 \\
0
\end{bmatrix} = 
\begin{bmatrix}
0 \cdot 1 + 1 \cdot 0 \\
1 \cdot 1 + 0 \cdot 1
\end{bmatrix} = 
\begin{bmatrix}
0 \\
1
\end{bmatrix} 
\\\\
X\ket{1} = 
\begin{bmatrix}
0 & 1 \\
1 & 0 \\
\end{bmatrix}
\begin{bmatrix}
0 \\
1
\end{bmatrix} = 
\begin{bmatrix}
0 \cdot 0 + 1 \cdot 1 \\
1 \cdot 0 + 0 \cdot 1
\end{bmatrix} = 
\begin{bmatrix}
1 \\
0
\end{bmatrix} \\
\end{gather*}
$$
And for general case:
$$

X\ket{\Psi} = 
\begin{bmatrix}
0 & 1 \\
1 & 0 \\
\end{bmatrix}
\begin{bmatrix}
\alpha \\
\beta
\end{bmatrix}
=
\begin{bmatrix}
0 \cdot \alpha + 1 \cdot \beta\\
1 \cdot \alpha + 0 \cdot \beta
\end{bmatrix}
= \beta \ket{0} + \alpha \ket{1} =
\begin{bmatrix}
\beta \\
\alpha
\end{bmatrix}
$$

# Ket-Bra representation

- ket represents the column vector
- bra represent the row vector

## Pauli gates (single-qubit gates)
