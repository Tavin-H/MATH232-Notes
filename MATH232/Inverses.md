<big><u>Vocabulary</u></big>
"Invertible" - A square matrix that has an inverse. Also called a non-singular.
"Singular Matrix" - A matrix with no inverse a.k.a. not Invertible
"Identity Matrix ($I$<sub>n</sub>)" - The $n$ x $n$ matrix with ones on the diagonal and zeros elsewhere. This acts as the multiplicative identity



<big><u>Definition</u></big>
B is the inverse of A if:
$$
BA = AB = I_{n}
$$
B can be written written as: $A$<sup>-1</sup>  



<big><u>Finding an Inverse</u></big>
Finding the inverse of a matrix $A$ is as simple as doing RREF with a slightly modified setup.

$$
\begin{align}

\text{let  }A = \begin{bmatrix}
1 & 2 & -1 \\
0 & 1 & -1 \\
-1 & 0 & -2
\end{bmatrix}
\end{align}
$$
To find $A$<sup>-1</sup> we setup an augmented matrix but with the identity matrix on the left side like so:
$$
\left[ \begin{matrix}
1 & 2 & -1  & | & 1 & 0 & 0\\
0 & 1 & -1  &|& 0 & 1 & 0\\
-1 & 0 & -2 & | & 0 & 0 & 1
\end{matrix}\right]
$$
Now we solve for RREF on the right side while still performing operations on the left
$$
\begin{align}
R_{3} = R_{3} + R_{1}\quad\quad\quad \\
\left[ \begin{matrix}
1 & 2 & -1  & | & 1 & 0 & 0\\
0 & 1 & -1  &|& 0 & 1 & 0\\
0 & 2 & -3 & | & 1 & 0 & 1
\end{matrix}\right] \\ \\

R_{3} = R_{3} - 2R_{2} \quad\quad\quad \\
\left[ \begin{matrix}
1 & 2 & -1  & | & 1 & 0 & 0\\
0 & 1 & -1  &|& 0 & 1 & 0\\
0 & 0 & -1 & | & 1 & -2 & 1
\end{matrix}\right]
 \\ \\ 
R_{2} = R_{2} - R_{3} \quad\quad\quad \\
\left[ \begin{matrix}
1 & 2 & -1  & | & 1 & 0 & 0\\
0 & 1 & 0  &|& -1 & 3 & -1\\
0 & 0 & -1 & | & 1 & -2 & 1
\end{matrix}\right] \\\\

R_{1} = R_{1} - 2R_{2} \quad\quad\quad \\
\left[ \begin{matrix}
1 & 0 & -1  & | & 3 & -6 & 2\\
0 & 1 & 0  &|& -1 & 3 & -1\\
0 & 0 & -1 & | & 1 & -2 & 1
\end{matrix}\right] \\\\

R_{1} = R_{1} - R_{3} \quad\quad\quad \\
R_{3} = -R_{3} \quad\quad\quad \\
\left[ \begin{matrix}
1 & 0 & 0  & | & 2 & -4 & 1\\
0 & 1 & 0  &|& -1 & 3 & -1\\
0 & 0 & 1 & | & -1 & 2 & -1
\end{matrix}\right] \\\\
\end{align}
$$
Notice that the identity matrix has now swapped sides. If you cannot make the identity matrix on the left side then $A$ is no invertible, that is, it has no inverse. This is known as a 'singular matrix'
The matrix on the right side is the Inverse of $A$ 
$$
\begin{align}
A = \begin{bmatrix}
1 & 2 & -1 \\
0 & 1 & -1 \\
-1 & 0 & -2
\end{bmatrix} \quad A^{-1} = \begin{bmatrix}
2 & -4 & 1 \\
-1 & 3 & -1 \\
-1 & 2 & -1
\end{bmatrix}
\end{align}
$$
You can check your answer by multiplying $A$ by $A$<sup>-1</sup> you should get the Identity Matrix
$$
\begin{bmatrix}
1 & 2 & -1 \\
0 & 1 & -1 \\
-1 & 0 & -2
\end{bmatrix}\begin{bmatrix}
2 & -4 & 1 \\
-1 & 3 & -1 \\
-1 & 2 & -1
\end{bmatrix} = \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0  \\
0 & 0 & 1
\end{bmatrix}
$$



<big><u>Properties of Inverses</u></big>
1. $(A^{-1})^{-1}$ = $A$
2. $(tA)^{-1}$ = $\frac{1}{2}A^{-1}$
3. $(AB)^{-1}$ = $B^{-1}A^{-1}$
4. $(A^T)^{-1}$ = $(A^{-1})^T$
*Note:* $A^T$ is the [[Transpose]] of A



<big><u>Formula for a 2x2 Matrix</u></big>
$$
\begin{align}
\text{let } A = \begin{bmatrix}
a & b \\
c & d
\end{bmatrix} \\
 \\
A^{-1} = \frac{1}{ad -bc}\begin{bmatrix}
d & -b \\
-c & a
\end{bmatrix}
\end{align}
$$
*Note:* Good luck remembering that lol
*Note:* If $ad-bc = 0$, the matrix is not invertible



<big><u>The Invertible Matrix Theorem</u></big>
All  these statements are equivalent, so if one is true, all are true. If one is false, all are false.
- $A$ is an Invertible matrix
- RREF of $A$ is I<sub>n</sub>
- Rank of $A$ is $n$ 
- The only solution of $A\vec{x} = \vec{0}$ is the trivial solution $\vec{x} = \vec{0}$.
- The nullspace is {$\vec{0}$}
- $A^T$ is an Invertible matrix
- The determinant of $A$ is non-zero
