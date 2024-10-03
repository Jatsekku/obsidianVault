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
- relation between bra and ket notion is as follows: 
$$
\bra{\Psi} = \ket{\Psi}^{\dagger}
$$
- $\ket{0}$ and $\ket{1}$ are normalized and orthogonal to each other - so it forms orthonormal basis. Due to this fact:
$$
\begin{gather*}
\braket{0|0} = \braket{1|1} = 1 \\\\
\braket{0|1} = \braket{1|0} = 0
\end{gather*}
$$
## Pauli gates (single-qubit gates)

## X gate
$$
\begin{gather*}
X =
\begin{bmatrix}
0 & 1 \\
1 & 0 \\
\end{bmatrix} \\\\

X = \ket{0} \bra{1} + \ket{1}\bra{0} \\\\
\ket{0}\bra{1} =
\begin{bmatrix}
1 \\
0
\end{bmatrix}
\begin{bmatrix}
0 & 1
\end{bmatrix}
+
\begin{bmatrix}
0 \\
1
\end{bmatrix}
\begin{bmatrix}
1 & 0
\end{bmatrix}
= 
\begin{bmatrix}
0 & 1 \\
0 & 0
\end{bmatrix}
+
\begin{bmatrix}
0 & 0 \\
1 & 0
\end{bmatrix}
= \begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}
\end{gather*}
$$

applying X gate to basis state 0 can be expressed using Dirac notation only:
$$
\begin{gather*}
X\ket{0} = \left(\ket{0}\bra{1} + \ket{1}\bra{0}\right)\ket{0} =
\ket{0}\braket{1|0} + \ket{1}\braket{0|0} = \\ 
\ket{0} \left( \braket{1|0} \right) + \ket{1} \left( \braket{0|0}\right) =
\ket{0} \left( 0 \right) + \ket{1} \left( 1 \right) = \ket{1}
\end{gather*}
$$