To cover:
- Adding
- Subtracting
- Dot product
- Scalar Multiplication
- Line passing through given point with given vector
- Line passing between 2 points - related to above


<big><u>Finding vector between 2 points:</u></big>
If you are given 2 points, $P$ and $Q$, you can find the vector that points from $P$ to $Q$ and vice-versa
$$
\begin{align}
\overrightarrow{PQ} = Q-P \\
\overrightarrow{QP} = P-Q
\end{align}
$$
$$
P=(0, 0,-2) \quad Q =(2, -1, 3)
$$
$$
\begin{align}
\overrightarrow{PQ} = \begin{bmatrix}
2 \\
-1 \\
3\end{bmatrix} - \begin{bmatrix}
0 \\
0 \\
-2\end{bmatrix} = \begin{bmatrix}
2 \\
-1 \\
5
\end{bmatrix} \\
 \\
\overrightarrow{QP} = \begin{bmatrix}
0 \\
0 \\
-2\end{bmatrix} - \begin{bmatrix}
2 \\
-1 \\
3\end{bmatrix} = \begin{bmatrix}
-2 \\
1 \\
-5\end{bmatrix}
\end{align}
$$
*Note:* $\overrightarrow{PQ} = -\overrightarrow{QP}$



<big><u>Norm of a vector:</u></big>
Notation:
$$
\lvert \vec{n} \rvert = \sqrt{\vec{n} \cdot \vec{n} }
$$
Add example to find distance between 2 points