---
share: "true"
title: Gradient Based Optimization
---

[Link](https://www.youtube.com/watch?v=atXrbIY6iyQ) for the video of Gradient Based Optimization.

## Introduction

#### What is optimization?

Optimization is selecting the best element with some criterion. Optimization problem is maximizing or minimizing functions by choosing inputs.[^1]

> [!Example] Real-life Optimizations Example
>
> - Optimizing the design to maximize the performance.
> - Optimizing the recommendation algorithm to show best personalized advertisement.
> - Optimizing the factory to spend less time and money.

## Mathematical Optimization

This is just finding $x$ that maximizes or minimizes some function $f(x)$. It is easy for some simple functions, i.e. quadratic functions.

$$
f(x)= ax^2 + bx+c \quad (a>0)
$$

To find $x$ that minimizes function $f(x)$, we simply differentiate $f(x)$.

$$
f'(x)=2ax+b=0
$$

$f(x)$ is minimized when $x=-\frac{b}{2a}$.
However, we want to find parameter values that minimizes the _complex_ function, harder to differentiate symbolically.

## Gradient Based Optimization

### Observations

![[GBO-slope.png|250]]

Assume that global minimum is a only local minimum, and $x'$ is a value that makes $f(x)$ minimum.
Then, slope of the function $f(x)$ indicates where minimum exists.

- If slope $f'(x_0)$ is positive, it means $x' < x_0$.
- If slope $f'(x_0)$ is positive, it means $x_0 < x'$.

Therefore, whatever the value of $x_0$ is, $x_1 = x_0 - f'(x_0)$ will move value to the direction of $x'$.
We can do this iteratively, and expect that sequence $\{x_n\}$ will be converge to $x'$.

$$
x_{n+1} = x_n - f'(x_n)
$$

### Problem: To steep slope

If function is to steep, sequence $\{x_n\}$ can diverge. Therefore, we add one hyperparameter, learning rate $\alpha\ (0<\alpha<1)$. Hyperparameter is set before optimization algorithm.[^2]

$$
x_{n+1} = x_n - \alpha f'(x_n)
$$

### Problem: Local minimum

We assumed that global minimum is a only local minimum. However, general functions can have local minimum, which is not a global minimum.

> [!Definition]
> **Local minimum** is a smallest value in the given range.

With method we build in [[GBO#Problem To steep slope|previous chapter]], sequence can easily trapped into the local minimum.

#### Another Observation

![[GBO-physics.png|400]]

In this example, ball will go to global minimum due to inertia. Therefore, we can apply inertia to our formula.

---

[^1]: https://en.wikipedia.org/wiki/Mathematical_optimization
[^2]: https://en.wikipedia.org/wiki/Hyperparameter_(machine_learning)
