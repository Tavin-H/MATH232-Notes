
<big><u>Theory</u></big>
Given any vector $a$, we can think of this vector as a product of it's 2 components labeled: $a$<sub>x</sub> and $a$<sub>y</sub>
These vectors are connected by the definition:
$$
\vec{a} = \vec{a}_{x}+ \vec{a}_{y}
$$
Now we can use some functions that relate to this 

<big><u>Projection</u></big>
First, let's look at the standard notation of a projection function
$$
Proj_{\vec{n}}\vec{a}
$$
This equation will give us the $a$<sub>x</sub> component. 
*Note:* the '$x$'  doesn't necessarily mean that it's parallel to the x-axis, that is only the case if $n$ is parallel to the x-axis

Here is an example of projecting the vector v onto some normal vector n

$$
Proj_{\vec{n}}\vec{v} = \frac{\vec{n} \cdot \vec{v}}{\lvert \vec{n} \rvert^2 }\vec{n}
$$

<big><u>Perpendicular</u></big>
Here is the standard notation of a perpendicular function:
$$
Perp_{\vec{n}}\vec{a} = \vec{a} - Proj_{\vec{n}}\vec{a}
$$
This gives us the $a$<sub>y</sub> as can be seen from the equation:
$$
\begin{align}

\vec{a} = \vec{a}_{x} + \vec{a}_{y} \\
\vec{a} - \vec{a}_{x} = \vec{a}_{x} + \vec{a}_{y} - \vec{a}_{x} \\
\vec{a} - \vec{a}_{x} = \vec{a}_{y}
\end{align}
$$


<big><u>Applications</u></big>
Using these equations, we can find some calculations.
For example, with these variables:
$$
\begin{align}

P = (0, 0, -2) \\
plane: -4x_{1} + x_{2} - 3x_{3} =  0
\end{align}
$$
We can find the shortest distance between a point and a plane like so:
1. Find vector between some test point $Q$ <u>on the plane</u> and the given point $P$.
$$
\begin{align}

Q = (-2, 1, 2) \\
\overrightarrow{QP} = \vec{P} - \vec{Q}\\ = \begin{bmatrix}
0 \\
0 \\
-2\end{bmatrix} - \begin{bmatrix}
-2 \\
1 \\
-3\end{bmatrix}\\ = \begin{bmatrix}
2 \\
-1 \\
-4\end{bmatrix}
\end{align}
$$
2. Find normal vector of the plane (please refer to [[Normal Vector]] to do this)
$$
\begin{align}

 plane: -4x_{1} + x_{2} - 3x_{3} =  0\\
 \vec{n} = \begin{bmatrix}
-4 \\
1 \\
-3\end{bmatrix}
\end{align}
$$
3. Project the vector $QP$ onto the normal vector $n$
$$
Proj_{\vec{n}}\overrightarrow{QP} = \frac{\vec{n} \cdot \overrightarrow{QP}}{\lvert \vec{n} \rvert ^2}\vec{n} = \frac{3}{26}\begin{bmatrix}
-4 \\
1 \\
-3\end{bmatrix} = \begin{bmatrix}
-\frac{12}{26} \\
\frac{3}{26} \\
-\frac{9}{26}
\end{bmatrix}
$$
4. Find the norm of the resulting projected matrix (please refer to [[Basic Vector Operations]] to do this)
$$

\left|\left| \begin{bmatrix}
-\frac{12}{26} \\
\frac{3}{26} \\
-\frac{9}{26}
\end{bmatrix} \right|\right|  = \sqrt{\frac{9}{26}} = \frac{3}{\sqrt{ 26 }}
$$
