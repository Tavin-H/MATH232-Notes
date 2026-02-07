<u><big>Notation</big></u>
let A be an $n$ x $m$ matrix,
$$
f_{A}: \vec{x} \rightarrow A\vec{x}
$$
*Example 1.1:*
$$
\begin{align}
A=\begin{bmatrix}
-3 & 4 & -4 \\
-5 & 5 & 3
\end{bmatrix} \quad \vec{x} = \begin{bmatrix}
3 \\
5 \\
-6
\end{bmatrix}
\end{align}
$$
$$
A\vec{x} = \begin{bmatrix}
-3 & 4 & -4 \\
-5 & 5 & 3
\end{bmatrix} \begin{bmatrix}
3 \\
5 \\
-6
\end{bmatrix} = \begin{bmatrix}
35 \\
-8
\end{bmatrix}
$$
Please refer to [[Matrix Multiplication]] to perform this operation yourself.

We can write the mapping as a matrix using the coefficients like so:
$$
f_{A} = \begin{bmatrix}
-3x_{1} + 4x_{2} -4x_{3} \\
-5x_{1} + 5x_{2} + 3x_{3}
\end{bmatrix}
$$
using $x$ from Example 1.1 we solve like so
$$
\begin{bmatrix}
-3(3)+ 4(5)-4(-6) \\
-5(3)+5(5)+3(-6)
\end{bmatrix} = \begin{bmatrix}
35 \\
-8
\end{bmatrix}
$$

*Terminology:* the output of a linear mapping is called an "image"

Example 1.2:
"Find the images of the standard basis vectors under f<sub>A</sub>"
$$
f_{A}\begin{bmatrix}
1 \\
0 \\
0\end{bmatrix}, \quad f_{A}\begin{bmatrix}
0 \\
1 \\
0\end{bmatrix}, \quad f_{A}\begin{bmatrix}
0 \\
0 \\
1\end{bmatrix} = \begin{bmatrix}
-3 \\
-5\end{bmatrix}, \begin{bmatrix}
4 \\
5\end{bmatrix}, \begin{bmatrix}
-4 \\
3\end{bmatrix}
$$
*Note:* the images of the standard basis vectors will result in the columns of $A$



<u><big>Standard Matrix Mapping</big></u>
let $L$ be defined as:

$$
\begin{align}
L(x_{1}, x_{2}, x_{3}) = (x_{1} - 5x_{2}, \ 3x_{2}, \ 6x_{1} - 8x_{2}) = (y_{1}, y_{2}, y_{3})
\end{align}
$$
Where $y$<sub>1</sub> to $y$<sub>3</sub> are the output components of the mapping
using the coefficients from $L$ we can make a vector for $x$<sub>1</sub> to $x$<sub>3</sub>

first write the column of $x$<sub>1</sub>: there is 1 $x$<sub>1</sub> in $y$<sub>1</sub>, none in $y$<sub>2</sub>, and 6 in $y$<sub>3</sub>
now column of $x$<sub>2</sub>: there are -5 in $y$<sub>1</sub>, 3 in $y$<sub>2</sub>, and -8 in $y$<sub>3</sub>
lastly, the column of $x$<sub>3</sub>: note this variable does not appear in any of the calculations so this column is all zeros.
Now combine all the columns into one matrix:
$$
\begin{bmatrix}
1 \\
0 \\
6\end{bmatrix},
\begin{bmatrix}
-5 \\
3 \\
-8\end{bmatrix}, \begin{bmatrix}
0 \\
0 \\
0\end{bmatrix} = \begin{bmatrix}
1 & -5 & 0 \\
0 & 3 & 0 \\
6 & -8 & 0
\end{bmatrix}
$$
This is the Standard Matrix Mapping



<u><big>Domain & Codomain</big></u>
let $A$ be a matrix with $m$ rows and $n$ columns
$$
\begin{bmatrix}
-3 & 4 & -4 \\
-5 & 5 & 3
\end{bmatrix}
$$
The domain of $A$ is R<sup>n</sup> in this case: R<sup>3</sup>
The codomain of $A$ is R<sup>m</sup> in this case: R<sup>2</sup>
$$
f_{A}: R^n \rightarrow R^m
$$
This can be seen from Example 1.1 in Notation
*Remember:* domain = columns, codomain = rows.



<u><big>Linear Mapping</big></u>
A linear mapping is defined as:
$$
f_{A}(\vec{x} + \vec{y}) = f_{A}(\vec{x}) + f_{A}(\vec{y})
$$
This can also be applied to any multiple of $x$ and $y$ like so:
$$
f_{A}(t\vec{x} + s\vec{y}) = tf_{A}(\vec{x}) + sf_{A}(\vec{y})
$$



<big><u>Composition of Mappings</u></big>
Mapping functions can be composed like so:
$$
f_{A} \circ f_{B} = BA
$$
For a composition to be defined, the domain of B must match the codomain of A. 
e.g. if $B$ is an $n$ x $m$  matrix, then $A$ must be an $m$ x $p$ matrix

Example of a defined composition:
$$
\begin{align}

 A = \begin{bmatrix}
0 & 2 & 1 \\
0 & 0 & -1
\end{bmatrix} \quad
B = \begin{bmatrix}
3 & -1
\end{bmatrix}  \\ \\
f_{A} \circ f_{B} = BA = \begin{bmatrix}
3 & -1
\end{bmatrix}\begin{bmatrix}
0 & 2 & 1 \\
0 & 0 & -1
\end{bmatrix}
\end{align}
$$
Example of an undefined composition:
$$
\begin{align}

A = \begin{bmatrix}
3 & 1 \\
0 & 1\end{bmatrix} \quad B= \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix} \\
 \\
f_{A} \circ f_{B} = BA = \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix} \begin{bmatrix}
3 & 1 \\
0 & 1\end{bmatrix}
\end{align}
$$
The domain of B is 3 and the codomain of A is 2 so the composition is <u>Not defined</u>
This is because of the rules of [[Matrix Multiplication]].



<u><big>Inverse Linear Mappings</big></u>
If a linear mapping $T: R^n \to R^n$ is associated with an invertible matrix A, then the mapping for itself is Invertible. The inverse mapping $T^{-1}$ 'undoes' the action of $T$. The standard matrix for $T^{-1}$ is simply $A^{-1}$.
Example:
$$
\begin{align}

L(x_{1}, x_{2}) = (x_{A} + 2x_{2}, -x_{1} + 3x_{2}) \\ \\
A = \begin{bmatrix}
1 & 2 \\
-1 & 3
\end{bmatrix} \quad\quad\quad\quad \\ \\
[L^{-1}] = \begin{bmatrix}
\frac{3}{5} & -\frac{2}{5} \\
\frac{1}{5} & \frac{1}{5}
\end{bmatrix}\quad\quad\quad
\end{align}

$$
(please refer to [[Inverses]] to do this operation yourself)
