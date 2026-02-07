<big><u>Row Space</u></big>
To find the basis of a Row space, first take the [[RREF]] of the matrix
$$
\begin{bmatrix}
1 & 2 & -1 & 4 \\
0 & 3 & 1 & 0 \\
3 & 6 & -3 & 12\end{bmatrix} = \begin{bmatrix}
1 & 2  & -1 & 4 \\
0 & 3 & 1 & 2  \\
0 & 0 & 0 & 0
\end{bmatrix} = \begin{bmatrix}
1 & 2 & -1 & 4 \\
0 & 1 & \frac{1}{3} & 0 \\
0 & 0 & 0 & 0 \end{bmatrix} = \begin{bmatrix}
1 & 0 & -\frac{5}{3} & 4 \\
0 & 1 & \frac{1}{3} & 0 \\
0 & 0 & 0 & 0
\end{bmatrix}
$$
Any rows in RREF form with a pivot column will be in the Row space. In this case:
$$
Rowspace = \left\{\begin{bmatrix}
1 \\
0\\
-\frac{5}{3} \\
4\end{bmatrix}, \begin{bmatrix}
0 \\
1 \\
\frac{1}{3} \\
0
\end{bmatrix}\right\}
$$
<big><u>Column Space</u></big>
The Column Space has the same setup as Row Space by taking the RREF of an augmented matrix. However, how you interpret it differs. From the RREF:
$$\begin{bmatrix}
1 & 0 & -\frac{5}{3} & 4 \\
0 & 1 & \frac{1}{3} & 0 \\
0 & 0 & 0 & 0
\end{bmatrix}
$$
We see that columns 1 and 2 are pivot columns so we take columns 1 and 2 from the <u>Original</u> Matrix. So Column Space is:
$$
Columnspace = \left\{
\begin{bmatrix}
1 \\
0 \\
3\end{bmatrix}, \begin{bmatrix}
2 \\
3 \\
6
\end{bmatrix}
\right\}
$$
<big><u>Null Space</u></big>
looking at the RREF, solve for $x$<sub>1</sub> and $x$<sub>2</sub> in terms of the free variables:
let $x$<sub>3</sub> = $t$ and $x$<sub>4</sub> = $s$
$$
\begin{bmatrix}
x_{1} \\
x_{2} \\
x_{3} \\
x_{4}\end{bmatrix} = \begin{bmatrix}
\frac{5}{3}s-4t \\
-\frac{1}{3}s \\
s \\
t\end{bmatrix} = s\begin{bmatrix}
\frac{5}{3} \\
-\frac{1}{3} \\
1 \\
0\end{bmatrix} + t\begin{bmatrix}
-4 \\
0 \\
0 \\
1
\end{bmatrix}
$$
According to the rank nullity theorem, the rank of the matrix + the nullity of the matrix add up to the number of columns.
This can also be thought of as # of columns in Column Space + # of Columns in Null Space = # of Columns total.