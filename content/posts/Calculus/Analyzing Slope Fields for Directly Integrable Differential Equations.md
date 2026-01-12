---
title: "Analyzing Slope Fields for Directly Integrable Differential Equations"
---

## Introduction
We may be given a slope field without knowing the differential equation that produced it. So, what properties of a differential equation can we deduce from its slope field?

As an example, consider the slope field of the differential equation $y' = x^2(2 - x)$ shown below.

Now, imagine that we don't know which differential equation produced this slope field. Our goal, then, is to gather as much information as possible about the equation by referring only to its slope field.

When analyzing slope fields, it's often helpful to visualize a few of the solution curves, so let's sketch a few.

We can now make the following observations:

*   **First**, the solution curves have vertical symmetry. Therefore, the equation must be of the form $y' = f(x)$. Indeed, the equation $y' = x^2(2 - x)$ is of this form.
*   **Second**, notice that the solution curves have stationary points along the lines $x = 0$ and $x = 2$. This means that the right-hand side of our differential equation must evaluate to zero on these lines. Indeed, this is true of our equation.
*   **Third**, notice that the lines $x = 0$ and $x = 2$ split the plane into three regions. The slopes of the solution curves in each of these regions are summarized in the table below.

| Region | $x < 0$ | $0 < x < 2$ | $x > 2$ |
| :--- | :---: | :---: | :---: |
| **Slope** | $+$ | $+$ | $-$ |
| **Sign** | $+$ | $+$ | $-$ |

The equation $y' = x^2(2 - x)$ indeed exhibits this behavior. To see this a little more clearly, let $f(x) = x^2(2 - x)$. A sketch of this function is shown below.

The sign of $f(x)$ in the three regions agrees with the above table:
*   $f(x)$ is positive for $x < 0$ and $0 < x < 2$, and
*   $f(x)$ is negative for $x > 2$.

---

## Example: Identifying an Equation That Generates a Slope Field Using Stationary Points

**Which of the following equations could have generated the slope field shown above?**

I. $y' = \ln(x(x - 1))$
II. $y' = (x - 1)(x + 1)$
III. $y' = x + 1$

### EXPLANATION
Notice that the slopes of the slope field are horizontal along the lines $x = 0$ and $x = 1$, as shown above. Therefore, the right-hand side of the differential equation should evaluate to zero on both of these lines.

With that in mind, let's check each equation:

*   The equation $y' = \ln(x(x - 1))$ gives the required behavior. The right-hand side evaluates to zero at $x = 0$ and $x = 1$.
*   The equation $y' = (x - 1)(x + 1)$ does not give the required behavior. The right-hand side evaluates to zero at $x = 1$ and $x = -1$, but it also evaluates to zero when $x = -1$, which is not a behavior exhibited by our slope field.
*   The equation $y' = x + 1$ does not give the required behavior. The right-hand side does not evaluate to zero at both $x = 0$ and $x = 1$.

Therefore, the correct answer is "I only."

**KEY PREREQUISITES**
*   Using Differentiation to Calculate Critical Points
*   Slope Fields for Directly Integrable Differential Equations

---

## Question 1
The differential equation that generates the slope field shown above is given by $y' = (x - a)(x - b)$. Find the value of $a + b$.

a) 4
b) 3
c) -4
d) 2
e) -2

## Question 2
Which of the following equations could have generated the slope field shown above?

I. $y' = x(x - 2)(x + 1)$
II. $y' = (x - 2)(x + 1)$
III. $y' = x^2 + 1$

a) II and III only
b) III only
c) I and II only
d) II only
e) I only

---

## Example: Identifying an Equation That Generates a Slope Field Using the Sign of the Slopes

**The diagram shown above is the slope field for which of the following differential equations?**

I. $y' = -x(x^2 - 4)$
II. $y' = x(x^2 - 4)$
III. $y' = x(x^2 + 4)$

### EXPLANATION
Notice the following properties of the given slope field:

*   **First**, the slopes of the slope field are horizontal along the lines $x = -2$, $x = 0$, and $x = 2$. Therefore, the right-hand side of the differential equation should equal zero on both of these lines.
    
    Of the given equations, the only equations that satisfy this condition are the following:
    $$y' = -x(x^2 - 4)$$
    $$y' = x(x^2 - 4)$$

*   **Second**, the lines $x = -2$, $x = 0$, and $x = 2$ divide the plane into 4 regions. The sign of the slopes in each of the 4 regions is easily deduced by considering the behavior of the solution curves in these regions. This information is summarized in the following table:

| Region | $x < -2$ | $-2 < x < 0$ | $0 < x < 2$ | $x > 2$ |
| :--- | :---: | :---: | :---: | :---: |
| **Slope** | $+$ | $-$ | $+$ | $-$ |
| **Sign** | $+$ | $-$ | $+$ | $-$ |

Of the two remaining options, the only one that gives this behavior is:
$$y' = -x(x^2 - 4)$$

Therefore, the correct answer is "I only."

**KEY PREREQUISITE**
*   Solving Polynomial Inequalities Using the Sign Table Method

---

## Question 3
Which of the following equations could have generated the slope field shown above?

I. $y' = x - 2$
II. $y' = x(x - 2)$
III. $y' = x^2(x - 2)$

a) I and III only
b) II and III only
c) II only
d) III only
e) I only

## Question 4
The diagram shown above is the slope field for which of the following differential equations?

a) $y' = (x - 1)(x + 2)$
b) $y' = (x - 1)^2$
c) $y' = (x - 1)(x + 2)$
d) $y' = (x + 1)^2$
e) $y' = x(x - 1)(x + 2)$

*(Note: Options (a) and (c) appear identical in the source text; please check the specific signs in the original visualization if they differ).*

---

## Example: Identifying an Equation That Generates a Slope Field Using the Sign of the Slopes and Factoring

**Which of the following equations could have generated the slope field shown above?**

I. $y' = x^2 - 4$
II. $y' = x^3 - 4x^2 + 4x$
III. $y' = 4 - x^2$

### EXPLANATION
Notice the following properties of the given slope field:

*   **First**, the slope field is zero along the lines $x = -2$ and $x = 2$. Therefore, the right-hand side of the differential equation should evaluate to zero on both of these lines.
*   **Second**, the lines $x = -2$ and $x = 2$ divide the plane into 3 regions. The sign of the slopes in each of the 3 regions is easily deduced by considering the behavior of the solution curves in these regions. This information is summarized in the following table:

| Region | $x < -2$ | $-2 < x < 2$ | $x > 2$ |
| :--- | :---: | :---: | :---: |
| **Slope** | $+$ | $-$ | $+$ |
| **Sign** | $+$ | $-$ | $+$ |

With that in mind, let's consider each equation:

*   The equation **$y' = x^2 - 4 = (x - 2)(x + 2)$** gives the required behavior.
*   The equation **$y' = x^3 - 4x^2 + 4x = x(x - 2)^2$** does not give the required behavior. The right-hand side evaluates to zero at $x = 0$, but not at $x = -2$.
*   The equation **$y' = 4 - x^2 = -(x - 2)(x + 2)$** does not give the required behavior. The right-hand side evaluates to zero at $x = -2$ and $x = 2$, but the sign of the slopes in the required regions (summarized below) does not correspond to the given slope field.

| Region | $x < -2$ | $-2 < x < 2$ | $x > 2$ |
| :--- | :---: | :---: | :---: |
| **Slope** | $-$ | $+$ | $-$ |
| **Sign** | $-$ | $+$ | $-$ |

Therefore, the correct answer is "I only."

---

## Question 5
Which of the following equations could have generated the slope field shown above?

a) $y' = x^2 - 2x$
b) $y' = x^2 - 4x + 4$
c) $y' = 2x - x^2$
d) $y' = x - 2$
e) $y' = (x - 2)^2$

## Question 6
The diagram shown above is the slope field for which of the following differential equations?

a) $y' = x^3 - 2x$
b) $y' = x^2 - 2x$
c) $y' = x^3 + 2x$
d) $y' = x - 2$
e) $y' = (x - 2)^2$

---

## Example: Identifying an Equation That Generates a Slope Field Using Asymptotes

**Which of the following equations could have generated the slope field shown above?**

I. $y' = \frac{x}{x + 1}$
II. $y' = \frac{x^2}{x + 1}$
III. $y' = \frac{1}{x + 1}$

### EXPLANATION
Notice the following properties of the given slope field:

*   The solution curves have the vertical asymptote $x = -1$.
*   The slopes of the slope field become horizontal as $x \to \pm \infty$.
*   The slopes of the slope field are positive for $x > -1$ and negative for $x < -1$.

With that in mind, let's consider each equation:

*   The equation $y' = \frac{x}{x + 1}$ does not give the required behavior. The slopes of the slope field for this differential equation are positive for all $x \neq -1$.
*   The equation $y' = \frac{x^2}{x + 1}$ gives the required behavior. Notice that the right-hand side of this equation is positive for $x > -1$ and negative for $x < -1$. Also $y' \to \pm \infty$ as $x \to -1$.
*   The equation $y' = \frac{1}{x + 1}$ does not give the required behavior. Notice that
    $$\lim_{x \to \pm \infty} \frac{1}{x + 1} = 0$$
    Therefore, the slopes of the slope field for this differential equation do not become horizontal as $x \to \pm \infty$.

Therefore, the correct answer is "II only."

**KEY PREREQUISITES**
*   Limits at Infinity and Horizontal Asymptotes of Rational Functions
*   Solving Rational Inequalities

---

## Question 7
Which of the following equations could have generated the slope field shown above?

a) $y' = x(x - 2)$
b) $y' = \frac{x}{(x - 2)^2}$
c) $y' = \frac{1}{(x - 2)^2}$
d) $y' = \frac{x}{x - 2}$
e) $y' = \frac{1}{x - 2}$

## Question 8
Identify the differential equation that generated the slope field above.

a) $y' = \frac{x - 1}{x + 1}$
b) $y' = \frac{x^2}{x^2 - 1}$
c) $y' = \frac{1}{x - 1}$
d) $y' = \frac{1}{x^2 - 1}$
e) $y' = \frac{x^2}{x - 1}$