<u><big>Definition</big></u>
Let $A$ be an $m$ x $n$ matrix, and let $B$ be an $n$ x $p$ matrix. The product $AB$ is defined as the products of the rows from $A$ and the columns from $B$. 
This can be thought of as the matrix of dot products between elements of $A$'s row space and $B$'s column space.
See [[Basic Vector Operations]] and [[Special Subspaces]].

*Example 1:*
$$
\begin{align}
A=\begin{bmatrix}
a & b \\
c & d
\end{bmatrix} 
\quad B =\begin{bmatrix}
w & x\\
y & z \\
\end{bmatrix}
\quad AB=\begin{bmatrix}
aw+by & ax+bz\\
cw+dy & cx+dz\\
\end{bmatrix}
\end{align}
$$
<u><big>Properties</big></u>
Note that matrix multiplication only works if the number of columns in $A$ matches the number of rows in $B$. Because of this fact, matrix multiplication does not commute, meaning the product $AB$ is not necessarily the same as the product $BA$.

*Example 2:*
$$
\begin{align}
A=\begin{bmatrix}
a & b \\
c & d
\end{bmatrix} 
\quad B =\begin{bmatrix}
u & v\\
w & x\\
y & z\\
\end{bmatrix}
\quad AB=undefined
\end{align}
\quad BA=\begin{bmatrix}
ua+vc & ub+vd\\
wa+xc & wb+xd\\
ya+zc & yb+zd\\
\end{bmatrix}
$$
As a general rule, the product of an $m$ x $n$ matrix and an $n$ x $p$ matrix will be an $m$ x $p$ matrix.

Additionally, $AB = AC$ does **NOT** imply that $B = C$, this is a consequence of the lack of commutativity.

Finally, $AB = 0$ does **NOT** imply that $A = 0$ or $B = 0$.

Some properties that DO still hold include:

1. Associativity: $A(BC) = (AB)C$
2. **Left** Distributivity: $A(B+C) = AB + AC$
3. Linearity: $A(c\vec{u})=c(A\vec{u})$ and $A(\vec{u}+\vec{v})=A\vec{u}+A\vec{v}$
4. [[Transpose]] of a Product: $(AB)^T=B^T A^T$

<u><big>Identity Matrix</big></u>
The $n$ x $n$ **identity matrix**, denoted $I_n$, is the square matrix with ones on the main diagonal and zeros everywhere else.
$$
\begin{align}
I_n=\begin{bmatrix}
1 & 0 & \dots & 0\\
0 & 1 & \dots & 0\\
\vdots & \vdots & \ddots & \vdots\\
0 & 0 & \dots & 1\\
\end{bmatrix} 
\end{align}
$$
This is the multiplicative identity for matrix multiplication.
For any $m$ x $n$ matrix $A$, we have $I_mA=A=AI_n$.

*Example 3:*
$$
\begin{align}
A =\begin{bmatrix}
a & b\\
c & d\\
e & f\\
\end{bmatrix}
\quad I_3A=AI_2= \begin{bmatrix}
a & b\\
c & d\\
e & f\\
\end{bmatrix}
\end{align}
$$