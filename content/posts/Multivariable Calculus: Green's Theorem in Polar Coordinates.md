---
title: "Multivariable Calculus: Green's Theorem in Polar Coordinates"
date: 2026-01-12T21:24:23+11:00
draft: false
---

# Multivariable Calculus: Green's Theorem in Polar Coordinates

## Navigation
*   **Introduction**
*   Expressing a Line Integral Along a Circular Path as a Double Integral Using Green's Theorem
*   Expressing a Line Integral Along a Path as a Double Integral Using Green's Theorem
*   Evaluating a Line Integral Using Green's Theorem
*   **Prerequisites**
    *   [Calculating the Displacement of a Particle Using Integration]({{< ref "/posts/Calculating the Displacement of a Particle Using Integration" >}})
    *   Introduction to Green's Theorem

---

## Introduction

Suppose we want to evaluate the line integral

$$ \oint_C (e^x - x^2y) \, dx + (y + xy^2) \, dy $$

where $C$ is the unit circle $x^2 + y^2 = 1$, oriented counterclockwise.

Direct evaluation of this integral is likely to be a difficult task. However, we can make light work of this tricky integral using Green's theorem.

Recall that Green's theorem states the following:

$$ \oint_C P \, dx + Q \, dy = \iint_D \left(\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}\right) \, dA $$

In our case, the region $D$ and its boundary $C$ (shown below) satisfy the conditions of Green's theorem.

> *[Diagram: A unit circle on the x-y plane with region $D$ shaded blue and boundary $C$ oriented counterclockwise]*

Now, since
$$ P(x, y) = e^x - x^2y, \quad Q(x, y) = y + xy^2, $$

we obtain the partial derivatives
$$ \frac{\partial P}{\partial y} = -x^2, \quad \frac{\partial Q}{\partial x} = y^2. $$

Applying Green's theorem, we get
$$ \oint_C (e^x - x^2y) \, dx + (y + xy^2) \, dy = \iint_D (y^2 - (-x^2)) \, dA $$
$$ = \iint_D (x^2 + y^2) \, dA. $$

This double integral will be easier to evaluate if we switch to plane polar coordinates.

The region $D$ in $xy$-coordinates can be represented as the region $R$ in polar coordinates, given by
$$ \Delta = \{(r, \theta) : 0 \le r \le 1, \, 0 \le \theta \le 2\pi \}. $$

The change of variables formula for plane polar coordinates states that
$$ \iint_D f(x, y) \, dA = \iint_R f(r \cos \theta, r \sin \theta) r \, dr \, d\theta. $$

Finally, we can calculate our double integral by applying the change of variables, as follows:
$$ \iint_D (x^2 + y^2) \, dA = \int_0^{2\pi} \int_0^1 (r^2) r \, dr \, d\theta $$
$$ = \int_0^{2\pi} \int_0^1 r^3 \, dr \, d\theta $$
$$ = \int_0^{2\pi} \left[ \frac{r^4}{4} \right]_0^1 \, d\theta $$
$$ = \int_0^{2\pi} \frac{1}{4} \, d\theta $$
$$ = \frac{1}{4} (2\pi) $$
$$ = \frac{\pi}{2}. $$

---

### Example: Expressing a Line Integral Along a Circular Path as a Double Integral Using Green's Theorem

Given that
$$ \oint_C x^2 \, dx + (xy - \cos y) \, dy = \int_0^{2\pi} \int_0^2 [\text{MISSING}] \, dr \, d\theta, $$
where $F(x, y) = \langle x^2, xy - \cos y \rangle$ and $C$ is the circle $x^2 + y^2 = 4$ oriented counterclockwise, what is the missing part of the equation?

**EXPLANATION**

First, notice that we can rewrite our integral as
$$ \oint_C x^2 \, dx + (xy - \cos y) \, dy. $$

Green's theorem states that
$$ \oint_C P \, dx + Q \, dy = \iint_D \left(\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}\right) \, dA. $$

In our case, the region $D$ and its boundary $C$ satisfy the conditions of Green's theorem:

> *[Diagram: A circle with radius 2 centered at the origin, shaded blue]*

Since $P(x, y) = x^2$ and $Q(x, y) = xy - \cos y$, we obtain
$$ \frac{\partial Q}{\partial x} = y, \quad \frac{\partial P}{\partial y} = 0. $$

Applying Green's theorem, we get
$$ \oint_C x^2 \, dx + (xy - \cos y) \, dy = \iint_D (y - 0) \, dA = \iint_D y \, dA. $$

Now, notice that the region $D$ can be represented in polar coordinates as
$$ \Delta = \{(r, \theta) : 0 \le r \le 2, \, 0 \le \theta \le 2\pi \}. $$

The change of variables formula for plane polar coordinates states that
$$ \iint_D f(x, y) \, dA = \iint_R f(r \cos \theta, r \sin \theta) r \, dr \, d\theta. $$

Therefore, we can write our double integral as
$$ \iint_D y \, dA = \int_0^{2\pi} \int_0^2 (r \sin \theta) r \, dr \, d\theta $$
$$ = \int_0^{2\pi} \int_0^2 r^2 \sin \theta \, dr \, d\theta. $$

So, the missing expression is $r^2 \sin \theta$.

---

### Question 1

Given that
$$ \oint_C y^2 \, dx + x \, dy = \int_0^{2\pi} \int_0^1 [\text{MISSING}] \, dr \, d\theta, $$
where $C$ is the circle $x^2 + y^2 = 1$ oriented counterclockwise, what is the missing part of the equation?

*   (a) $r - r^2 \cos \theta$
*   (b) $1 - 2r \sin \theta$
*   (c) $r - 2r^2 \sin \theta$
*   (d) $r^2 \sin \theta - r \cos \theta$
*   (e) $r - r^2 \sin \theta$

**[Submit]**

---

### Question 2

Given that
$$ \oint_C \mathbf{F} \cdot d\mathbf{r} = \int_0^{2\pi} \int_0^3 [\text{MISSING}] \, dr \, d\theta, $$
where $\mathbf{F}(x, y) = \langle xy^2, x + e^{\cos y} \rangle$ and $C$ is the circle $x^2 + y^2 = 9$ oriented counterclockwise, what is the missing part of the equation?

*   (a) $r - r^2 \sin \theta$
*   (b) $r + r^2 \sin \theta$
*   (c) $r - r^3 \sin 2\theta$
*   (d) $e^{\cos \theta} - \sin^2 \theta$
*   (e) $r e^{\cos \theta} - r \sin^2 \theta$

**[Submit]**

---

### Example: Expressing a Line Integral Along a Path as a Double Integral Using Green's Theorem

> *[Diagram: A semi-circular region in the right half-plane ($x \ge 0$), bounded by the y-axis and an arc]*

Consider the path $O$ shown above and the vector field $\mathbf{F}(x, y) = \langle 3y + \ln(\sqrt{x+2}), x^{100} + 3x \rangle$.
Find a repeated integral in plane polar coordinates that's equivalent to $\oint_O \mathbf{F} \cdot d\mathbf{r}$.

**EXPLANATION**

First, notice that we can rewrite our integral as
$$ \oint_C -4y \, dx + (\ln(\sqrt{x+2}) + x) \, dy. $$
*(Note: The text in the explanation derivation seems to use a different vector field example than the prompt text above it. Based on the derivation steps visible:)*

Green's theorem states that
$$ \oint_C P \, dx + Q \, dy = \iint_D \left(\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}\right) \, dA. $$

In our case, the region $D$ and its boundary $O$ satisfy the conditions of Green's theorem:
> *[Diagram: Region $D$ shaded blue]*

Since $P(x, y) = -4y + \ln(\sqrt{x+2})$ and $Q(x, y) = x$, we obtain
*(Note: Derivation text obscured or inconsistent in snippet, but concludes with integral setup)*

Applying Green's theorem, we get
$$ \oint_C (-4y + \dots) \, dx + (x + \dots) \, dy = \iint_D (1 - (-4)) \, dA = \iint_D 5 \, dA. $$

Now, notice that the region $D$ can be represented in polar coordinates as
$$ \Delta = \{(r, \theta) : -\frac{\pi}{2} \le \theta \le \frac{\pi}{2}, \, 0 \le r \le 2 \}. $$

The change of variables formula for plane polar coordinates states that
$$ \iint_D f(x, y) \, dA = \iint_R f(r \cos \theta, r \sin \theta) r \, dr \, d\theta. $$

Therefore, we can write our double integral as
$$ \iint_D 5 \, dA = \int_{-\pi/2}^{\pi/2} \int_0^2 5r \, dr \, d\theta. $$

---

### Question 3

> *[Diagram: Right semi-circle region, radius 2]*

Consider the path $C$ shown above. Which of the following is equivalent to the line integral
$$ \oint_C (3y - e^{\cos x}) \, dx + (7x + \sqrt{y + 5}) \, dy? $$

*   (a) $\int_{-\pi/2}^{\pi/2} \int_0^2 2r \, dr \, d\theta$
*   (b) $\int_{-\pi/2}^{\pi/2} \int_0^2 4r \, dr \, d\theta$
*   (c) $\int_0^{\pi} \int_0^2 4r \, dr \, d\theta$
*   (d) $\int_{-\pi/2}^{\pi/2} \int_0^2 (r^3 - e^{\cos \theta}) \, dr \, d\theta$
*   (e) $\int_0^{\pi} \int_0^2 (r^3 - e^{\cos \theta})r \, dr \, d\theta$

**[Submit]**

---

### Question 4

> *[Diagram: Region in the 3rd quadrant bounded by unit circle arc and axes]*

Consider the path $C$ shown above. Given that $\mathbf{F}(x, y) = \langle x^2 \cos x + y^3, ye^{y+1} + x \rangle$, which of the following is equivalent to $\oint_C \mathbf{F} \cdot d\mathbf{r}$?

*   (a) $\int_{\pi}^{2\pi} \int_0^1 (r - \sin^2 \theta)r \, dr \, d\theta$
*   (b) $\int_{\pi}^{3\pi/2} \int_0^1 (r^2 - 3 \sin \theta) \, dr \, d\theta$
*   (c) $\int_{\pi}^{2\pi} \int_0^1 (1 - 3r^2 \sin^2 \theta) \, dr \, d\theta$
*   (d) $\int_{\pi}^{3\pi/2} \int_0^1 (1 - 3r^2 \sin^2 \theta)r \, dr \, d\theta$
*   (e) $\int_{\pi}^{3\pi/2} \int_0^1 (r^2 - 3 \sin \theta)r \, dr \, d\theta$

**[Submit]**

---

### Example: Evaluating a Line Integral Using Green's Theorem

> *[Diagram: Upper semi-circle region, radius 3]*

Evaluate $\oint_O (e^{x^2} - y^2) \, dx + (x^2 + e^{y^2}) \, dy$, where the path $O$ is shown above.

**EXPLANATION**

Green's theorem states that
$$ \oint_C P \, dx + Q \, dy = \iint_D \left(\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}\right) \, dA. $$

In our case, the region $D$ and its boundary $O$ satisfy the conditions of Green's theorem.

Now, since
$$ P(x, y) = e^{x^2} - y^2, \quad Q(x, y) = x^2 + e^{y^2}, $$
we obtain
$$ \frac{\partial P}{\partial y} = -2y, \quad \frac{\partial Q}{\partial x} = 2x. $$

Applying Green's theorem, we get
$$ \oint_C (e^{x^2} - y^2) \, dx + (x^2 + e^{y^2}) \, dy = \iint_D (2x - (-2y)) \, dA $$
$$ = \iint_D (2x + 2y) \, dA. $$

Now, notice that the region $D$ can be represented in polar coordinates as
$$ \Delta = \{(r, \theta) : 0 \le \theta \le \pi, \, 0 \le r \le 3 \}. $$

The change of variables formula for plane polar coordinates states that
$$ \iint_D f(x, y) \, dA = \iint_R f(r \cos \theta, r \sin \theta) r \, dr \, d\theta. $$

Finally, we can calculate our double integral, as follows:
$$ \int_0^{\pi} \int_0^3 [2(r \cos \theta) + 2(r \sin \theta)] r \, dr \, d\theta $$
$$ = \int_0^{\pi} \int_0^3 (2r^2 \cos \theta + 2r^2 \sin \theta) \, dr \, d\theta $$
$$ = \int_0^{\pi} \left[ \frac{2}{3}r^3 \cos \theta + \frac{2}{3}r^3 \sin \theta \right]_0^3 \, d\theta $$
$$ = \int_0^{\pi} (18 \cos \theta + 18 \sin \theta) \, d\theta $$
$$ = [18 \sin \theta - 18 \cos \theta]_0^{\pi} $$
$$ = (0 - (-18)) - (0 - 18) $$
$$ = 18 + 18 $$
$$ = 36. $$

---

### Question 5

Use Green's theorem to evaluate $\oint_C \mathbf{F} \cdot d\mathbf{r}$, where $\mathbf{F}(x, y) = \langle x^2y - \cos x, 4 - xy^2 \rangle$ and $C$ is the circle $x^2 + y^2 = 4$, oriented counterclockwise.

*   (a) $16\pi$
*   (b) $\frac{13\pi}{2}$
*   (c) $-8\pi$
*   (d) $-\frac{9\pi}{2}$
*   (e) $-20\pi$

**[Submit]**

---

### Question 6

> *[Diagram: Quarter circle region in the 1st quadrant, radius 1]*

Evaluate $\oint_C (\sqrt{x} - 4x^2y) \, dx + (e^y + 4xy^2) \, dy$, where the path $C$ is shown above.

*   (a) $4\pi$
*   (b) $8\pi$
*   (c) $2\pi$
*   (d) $-\frac{\pi}{2}$
*   (e) $-4\pi$

**[Submit]**