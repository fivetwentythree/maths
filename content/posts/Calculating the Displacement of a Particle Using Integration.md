---
title: "Calculating the Displacement of a Particle Using Integration"
date: 2026-01-12T21:24:23+11:00
---
## Calculating the Displacement of a Particle Using Integration

### Introduction

The **total displacement** $d$ of a particle over the time interval $t \in [a, b]$ is the difference in the position of the particle between $t = a$ and $t = b$.

$$d = s(b) - s(a)$$

Now, the fundamental theorem of calculus states that

$$d = s(b) - s(a) = \int_{a}^{b} s'(t) \, dt$$

and since $s'(t) = v(t)$, we can find the total displacement of a particle by integrating the velocity:

$$d = s(b) - s(a) = \int_{a}^{b} v(t) \, dt$$

To summarize, the total displacement of a particle over the time interval $t \in [a, b]$ can be found by integrating the velocity $v(t)$ over the time interval $t \in [a, b]$.

$$d = \int_{a}^{b} v(t) \, dt$$

---

### Example: Finding the Total Displacement of a Particle Given Its Velocity

A particle $P$ moves along the $x$-axis and its velocity at time $t$ is given by $v(t) = 2t + 3t^2$. What is the total displacement of the particle between $t = 1$ and $t = 3$?

**EXPLANATION**

We find the total displacement by calculating the definite integral of the velocity.

Let $d$ be the total displacement. Then, we have

$$
\begin{aligned}
d &= \int_{1}^{3} (2t + 3t^2) \, dt \\
&= [t^2 + t^3]_{1}^{3} \\
&= (3^2 + 3^3) - (1^2 + 1^3) \\
&= (9 + 27) - (1 + 1) \\
&= 36 - 2 \\
&= 34.
\end{aligned}
$$

So the total displacement between $t = 1$ and $t = 3$ is **34**.

**KEY PREREQUISITE**
*   The Sum and Constant Multiple Rules for Definite Integrals

---

### Question 1
*A scientific calculator is required to answer this question.*

A particle $P$ moves along the $x$-axis and its velocity at time $t$ is given by $v(t) = 6t^2 - 2t$. What is the total displacement of the particle between $t = 1$ and $t = 4$?

a) 4
b) 88
c) 111
d) 148
e) 92

---

### Question 2
*A scientific calculator is required to answer this question.*

A particle $P$ moves along the $x$-axis and its velocity at time $t$ is given by $v(t) = 12t^2 - 4t$. What is the total displacement of the particle between $t = 0$ and $t = 3$?

a) 72
b) 0
c) 90
d) 96
e) 68

---

### Example: Finding the Final Position of a Particle

A particle $P$ moves along the $x$-axis and its velocity at time $t > 0$ is given by $v(t) = 6t^2 + 4t$. At time $t = 2$ the particle is located at the position $x = -20$. What is the position of the particle at time $t = 4$?

**EXPLANATION**

The position of the particle at $t = 4$ is equal to its position at $t = 2$ plus the total displacement over $t \in [2, 4]$. Therefore, we can calculate it as follows:

$$s(4) = s(2) + \int_{2}^{4} v(t) \, dt$$

Carrying out the computations, we get

$$
\begin{aligned}
s(4) &= -20 + \int_{2}^{4} (6t^2 + 4t) \, dt \\
&= -20 + [2t^3 + 2t^2]_{2}^{4} \\
&= -20 + ((2(4)^3 + 2(4)^2) - (2(2)^3 + 2(2)^2)) \\
&= -20 + ((128 + 32) - (16 + 8)) \\
&= -20 + (160 - 24) \\
&= -20 + 136 \\
&= 116.
\end{aligned}
$$

So the position of the particle at $t = 4$ is **116**.

**KEY PREREQUISITE**
*   The Integral as an Accumulation Function

---

### Question 3
*A scientific calculator is required to answer this question.*

A particle $P$ moves along the $x$-axis and its velocity at time $t \ge 0$ is given by $v(t) = e^{t/3} - 1$. At time $t = 0$ the particle is located at the position $x = e + 1$. What is the position of the particle at time $t = 3$?

a) $x = 4e^3$
b) $x = 3e^3 - e$
c) $x = e - 1$
d) $x = 4e - 5$
e) $x = 3e - 1$

---

### Question 4
*A scientific calculator is required to answer this question.*

A particle $P$ moves along the $x$-axis and its velocity at time $t > 0$ is given by $v(t) = 4t + 3t^2$. At time $t = 1$ the particle is located at the position $x = 12$. What is the position of the particle at time $t = 4$?

a) 105
b) 97
c) 100
d) 93
e) 92

---

### Example: Finding the Final Position of a Particle Given a Velocity-Time Graph

The graph above shows the velocity of an object moving in a straight line along the $x$-axis. At time $t = 2$ the particle is located at the position $x = -1$. What is the position of the particle at time $t = 5$?

**EXPLANATION**

The position of the particle at $t = 5$ is equal to its position at $t = 2$ plus the total displacement over $t \in [2, 5]$. Therefore, we can calculate it as follows:

$$x(5) = x(2) + \int_{2}^{5} v(t) \, dt$$

We are told that $x(2) = -1$, and we can compute the integral $\int_{2}^{5} v(t) \, dt$ by finding the signed area under the graph from $t = 2$ to $t = 5$. Computing the signed area, we get

$$\int_{2}^{5} v(t) \, dt = 6.$$

Therefore,

$$x(5) = -1 + 6 = 5$$

So the position of the particle at $t = 5$ is $x = 5$.

**KEY PREREQUISITES**
*   Calculating the Definite Integral of a Function Given Its Graph
*   Calculating Distance From a Speed-Time Graph

---

### Question 5
The graph above shows the velocity of an object moving in a straight line along the $x$-axis. At time $t = 1$ the particle is located at the position $x = 2$. What is the position of the particle at time $t = 7$?

a) 4
b) 8
c) 2
d) 6
e) 7

---

### Question 6
The graph above shows the velocity of an object moving in a straight line along the $x$-axis. At time $t = 0$ the particle is located at the position $x = 6$. What is the position of the particle at time $t = 3$?

a) 11
b) 20
c) 8
d) 14
e) 12

