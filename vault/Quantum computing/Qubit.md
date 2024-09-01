# Matrix representation
$$
\begin{bmatrix}
\alpha \\
\beta
\end{bmatrix}
$$
- vector is normalized: $$ |\alpha|^2 + |\beta|^2 = 1 $$
# Dirac notation

$$
\ket{0} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \space
\ket{1} =\begin{bmatrix} 0 \\ 1 \end{bmatrix} 
$$
$$
\ket{\Psi} =
\begin{bmatrix}
\alpha \\ \beta
\end{bmatrix}
= \alpha\ket{0} + \beta\ket{1}
$$
## commonly used ket symbols
- Basis states:
$$
\ket{0} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \space
\ket{1} =\begin{bmatrix} 0 \\ 1 \end{bmatrix} 
$$
- others:
$$\ket{+} = \frac{1}{\sqrt{2}} \left( \ket{0} + \ket{1} \right)$$
$$\ket{-} = \frac{1}{\sqrt{2}} \left( \ket{0} - \ket{1} \right)$$
$$\ket{i} = \frac{1}{\sqrt{2}} \left( \ket{0} + i\ket{1} \right)$$
$$\ket{-i} = \frac{1}{\sqrt{2}} \left( \ket{0} - i\ket{1} \right)$$
## Relative phase
Probability amplitudes of quantum state are expressed as two complex numbers:
$$
\ket{\Psi} = 
\begin{bmatrix}
\alpha \\ \beta
\end{bmatrix}
= 
\begin{bmatrix}
Re(\alpha) + Img(\alpha)i \\
Re(\beta) + Img(\beta)i
\end{bmatrix}
= 
\begin{bmatrix}
|\alpha| e^{i\theta_{\alpha}} \\
|\beta| e^{i\theta_{\beta}}
\end{bmatrix}

$$
relative phase of $\Psi$ is defined as:
$$
\theta_r = \theta_{\alpha} - \theta_{\beta} 
$$
### Example:
$$
\begin{gather*}
\ket{\Psi} = \frac{1 + i}{2} \ket{0} + \frac{1-i}{2} \ket{1} = 
\frac{1 + i}{2}
\begin{bmatrix}
1 \\ 0
\end{bmatrix}
+
\frac{1 - i}{2}
\begin{bmatrix}
0 \\ 1
\end{bmatrix}
=
\begin{bmatrix}
{\frac{1}{2} + \frac{1}{2}i} \\
{\frac{1}{2} - \frac{1}{2}i}
\end{bmatrix} = \\
\begin{bmatrix}
{\sqrt{{\frac{1}{2}}^2 + {\frac{1}{2}}^2}}e^{i\cdot \mathrm{atan2}(\frac{1}{2}, \frac{1}{2})} \\
{\sqrt{{\frac{1}{2}}^2 + {\frac{1}{2}}^2}}e^{i\cdot \mathrm{atan2}(\frac{1}{2}, -\frac{1}{2})}
\end{bmatrix} =
\begin{bmatrix}
\frac{1}{\sqrt{2}} e^{\frac{\pi}{4}i} \\
\frac{1}{\sqrt{2}} e^{-\frac{\pi}{4}i}
\end{bmatrix}
\end{gather*}
$$
as we can se:
$$
\theta_{\alpha} = \frac{\pi}{4}, \space \theta_{\beta} = - \frac{\pi}{4}
$$
so:
$$
\theta_{r} = \theta_{\alpha} - \theta_{\beta} = \frac{\pi}{4} - \left( -\frac{\pi}{4}\right) = \frac{\pi}{4} + \frac{\pi}{4} = \frac{\pi}{2}
$$
## Global phase
$$
e^{i\theta_{g}} \ket{\Psi} = e^{i\theta_{g}} \left( \alpha \ket{0} + \beta \ket{1} \right)
$$
$\theta_g$ - global phase

- it doesn't change the quantum state - because it is not influencing the relative phase of state. 
- Due to this fact it's also called unobservable or hidden phase.
