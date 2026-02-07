<big><u>Notation</u></big>
The transpose of a matrix $A$ is simply:
$$
A^T
$$

<big><u>Finding the Transpose</u></big>
To find the transpose of a given matrix, simply make the first column into the first row, second column into the second row... etc.
Example:
$$
\begin{align}

A = \begin{bmatrix}
5 & 0 & -2 \\
6 & 1 & 3
\end{bmatrix} \quad\quad A^T =\begin{bmatrix}
5 & 6 \\
0 & 1 \\
-2 & 3
\end{bmatrix}
\end{align}
$$
This transformation can be shown as
$$
[A^T]_{ij} = [A]_{ji}
$$
*Note:* if $A$ is an $n$ x $m$ matrix, then $A^T$ is an $m$ x $n$ matrix.


<big><u>Some Extra Info</u></big>
$(A^T)^T = A$ 

if $A^T = A$, then $A$ is symmetric (link to wherever symmetry is explained)
