Normal Vector of a Line:
Use the coefficients of the variables to form a vector:
$$
-2x_{1}+ 3x_{2} = 0 \implies
\begin{bmatrix}
-2 \\
3
\end{bmatrix}
$$
<big><u>Normal vector of a plane</u></big>
let $P$ be the plane:
$$
P = -x +8y -2z = -11
$$
The normal vector of this plane is the vector formed by the coefficients of the $x$, $y$, and $z$ components. like so:
$$
\vec{n} = \begin{bmatrix}
-1 \\
8 \\
-2
\end{bmatrix}
$$
*Note:* the value on the RHS has no effect on the normal vector

<big><u>Normal vector of a plane 2</u></big>
when given a vector equation of a plane, the calculation becomes a little harder.
This time let $P$ be the plane:
$$
\vec{x} = s\begin{bmatrix}
2 \\
3 \\
1\end{bmatrix} + t\begin{bmatrix}
1 \\
-3 \\
-1\end{bmatrix}
$$
the idea is that the plane is defined by 2 lines, and the normal vector is going to be perpendicular to both of these lines. That is,
$$
\begin{align}

\vec{n} \cdot \begin{bmatrix}
2 \\
3 \\
1\end{bmatrix} = 0, \quad \vec{n} \cdot \begin{bmatrix}
1 \\
-3 \\
-1\end{bmatrix} = 0
\end{align}
$$
*Note:* if there is a constant term (a vector with no variable), then you can just ignore it

If we write $n$ as a vector of arbitrary numbers, we can write the dot products as a system of linear equations:
$$
\begin{align}

\vec{n} = \begin{bmatrix}
A \\
B \\
C
\end{bmatrix} \quad \rightarrow \quad\begin{bmatrix}
A \\
B \\
C\end{bmatrix} \cdot \begin{bmatrix}
2 \\
3 \\
1\end{bmatrix} = 0 \quad \begin{bmatrix}
A \\
B \\
C\end{bmatrix} \cdot \begin{bmatrix}
1 \\
-3 \\
-1\end{bmatrix} = 0
\end{align}
$$
evaluating we get:
$$
\begin{align}
2A + 3B + C = 0 \\
A -3B -C = 0
\end{align}
$$
Solving the system we get:
first equation - second equation -> A=0
$$
\begin{align}

2A + 3B + C = 0 \\
-(A -3B -C = 0) \\
A = 0
\end{align}
$$
Then:
$$
\begin{align}
3B + C = 0 \\
-3B -C = 0
\end{align}
$$
These are the same equation so $C = -3B$ and obviously $C = C$
Now that we have all the values of $A, B$ and $C$, we can pick a convenient value for C to solve:
$$
\vec{n} = \begin{bmatrix}
0 \\
-3B \\
C\end{bmatrix} \quad C = 1 \rightarrow \vec{n} = \begin{bmatrix}
0 \\
-3 \\
1
\end{bmatrix}
$$


<big><u>Normal vector of a plane 3</u></big>
If you are given 3 points then the process is the same as Method 2 however there is a bit of setup first:
$$
\begin{align}

\end{align}
$$

$$

$$