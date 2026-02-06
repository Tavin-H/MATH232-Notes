
<big>Method 1</big>
"Reflection across a given line"
use e<sub>1</sub> and e<sub>2</sub> to find the matrix columns individually
$$
\begin{align}

\vec{e_{1}} = \begin{bmatrix}
1 \\
0
\end{bmatrix} \quad \vec{e_{2}} = \begin{bmatrix}
0 \\
1
\end{bmatrix} \\

\end{align}

$$
$$
Col(H)_{1} = \vec{e_{1}} -2\frac{(\vec{e_{1}} \cdot\vec{n})}{\lvert \vec{n} \rvert^2 }\vec{n}
$$
Repeat with e<sub>2</sub> to find Col(H)<sub>2</sub>
see [[Normal Vector]] to find n
*Note:*
$$
\begin{align}

\vec{e_{1}} \cdot \vec{n} = \vec{n}_{1} \\
\vec{e_{2}} \cdot \vec{n} = \vec{n_{2}} \\
 \\
\frac{\vec{e_{1}} \cdot\vec{n}}{\lvert \vec{n} \rvert^2 } = Proj_{\vec{n}}(\vec{e_{1}})
\end{align}
$$
This may simplify the calculation or make it easier to remember
see [[Projection]] to calculate Proj<sub>n</sub>(x)

<big>Method 1.5 </big>
This is a simplification of Method 1. However, in my opinion it's a bit harder to memorize:
$$
\begin{align}
line = ax_{1}+bx_{2}  \\ \\

H = \frac{1}{a^2 + b^2}\begin{bmatrix}
b^2-a^2 & -2ab \\
-2ab & a^2-b^2
\end{bmatrix}
\end{align}
$$

<big>Method 2. </big>
"Reflection across an angle"
if an angle in radians is given then you can use the standard 2x2 rotation matrix:
$$
Ref(x) = x\begin{bmatrix}
\cos \theta & -\sin \theta \\
\sin \theta & \cos \theta
\end{bmatrix}
$$

