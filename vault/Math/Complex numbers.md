## Algebraic form
 $$z = a + ib$$
Addition: 
$$
\begin{gathered}
z_{1} = a_{1} + ib_{1} \\
z_{2} = a_{2} + ib_{2} \\\\
z_{1} + z_{2} = (a_{1} + a_{2}) + i(b_{1} + b_{2})
\end{gathered}
$$

Multiplication:
$$
\begin{gathered}
z_{1} = a_{1} + ib_{1} \\
z_{2} = a_{2} + ib_{2} \\\\
z_{1} \cdot z_{2} = a_{1}a_{2} + ia_{1}b_{2} + ia_{2}b_{1} + i^2b_{1}b_{2} = (a_{1}a_{2} - b_{1}b_{2}) + i(a_{1}b_{2} + a_{2}b_{1})
\end{gathered}
$$
Conjugate:
$$
\begin{gathered}
z = a + ib \\
{z}^{*} = a - ib \\
\end{gathered}
$$
Division:
$$
\begin{gathered}
z_{1} = a_{1} + ib_{1} \\
z_{2} = a_{2} + ib_{2} \\\\
\frac{z_{1}}{z_{2}}  = \frac{z_{1} \cdot {z_{2}}^{*}}{z_{2} \cdot {z_{2}}^{*}}= \frac{(a_{1} + ib_{1})(a_{2} - ib_{2})}{(a_{2} + ib_{2})(a_{2} - ib_{2})} = \frac{(a_{1}a_{2} - b_{1}b_{2}) + i(a_{1}b_{2} + a_{2}b_{1})}{{a_{2}}^2 + {b_{2}}^2}
\end{gathered}
$$
Module:
$$|z| = \sqrt{a^2 + b^2}$$
## Trigonometric form

$$ z = r (cos(\theta) + isin(\theta)) $$

Multiplication:
$$
\begin{gathered}
z_{1} = r_{1}(cos(\theta_{1}) + isin(\theta_{1})) \\
z_{2} = r_{2}(cos(\theta_{2}) + isin(\theta_{2})) \\\\
z_{1} \cdot z_{2} = [r_{1}(cos(\theta_{1}) + isin(\theta_{1}))][r_{2}(cos(\theta_{2}) + isin(\theta_{2}))] = \\
[r_1cos(\theta_1) + ir_1sin(\theta_1)][r_2cos(\theta_2) + ir_2sin(\theta_2)] = \\
r_{1}r_{2}cos(\theta_{1})cos(\theta_2) + ir_{1}r_{2}cos(\theta_{1})sin(\theta_{2}) + ir_{1}r_{2}sin(\theta_{1})cos(\theta_{2}) + i^{2}r_{1}r_{2}sin(\theta_{1})sin(\theta_{2}) = \\
r_{1}r_{2}cos(\theta_{1})cos(\theta_{2}) - r_{1}r_{2}sin(\theta_{1})sin(\theta_{2}) + i(r_{1}r_{2}cos(\theta_{1})sin(\theta_{2}) + r_{1}r_{2}sin(\theta_{1})cos(\theta_{2})) = \\
r_{1}r_{2}(cos(\theta_{1})cos(\theta_{2}) - sin(\theta_{1})sin(\theta_{2})) + ir_{1}r_{2}(cos(\theta_{1})sin(\theta_{2}) + sin(\theta_{1})cos(\theta_{2}))) = \\\\

\text{Using following trig identities:}\\
sin(\theta_{1} + \theta_{2}) = sin(\theta_{1})cos(\theta_{2}) + cos(\theta_{1})sin(\theta_2) \\
cos(\theta_{1} + \theta_{2}) = cos(\theta_{1})cos(\theta_{2}) - sin(\theta_{1})sin(\theta_{2}) \\
\text{we get:} \\\\

= r_{1}r_{2}(cos(\theta_{1} + \theta_{2}) + isin(\theta_{1} + \theta_{2}))
\end{gathered}
$$
Conjugate:
$$
\begin{gathered}
z = r (cos(\theta) + isin(\theta)) \\
{z}^{*} = r (cos(\theta) - isin(\theta)) \\
\end{gathered}
$$
Module:
$$|z| = r$$
## Exponential form
$$ z = re^{i\theta} $$
Multiplication:
$$
\begin{gathered}
z_{1} = r_{1}e^{i\theta_{1}} \\
z_{2} = r_{2}e^{i\theta_{2}} \\\\
z_{1} \cdot z_{2} = r_{1}e^{i\theta_{1}} \cdot r_{2}e^{i\theta_{2}} = r_{1}r_{2}e^{i(\theta_{1} + \theta_{2})}
\end{gathered}
$$
Conjugate:
$$
\begin{gathered}
z = re^{i\theta} \\
{z}^{*} = re^{-i\theta} \\
\end{gathered}
$$
Module:
$$|z| = r$$
## General properties
$${z}^{*}z = z{z}^{*} = r^{2}$$