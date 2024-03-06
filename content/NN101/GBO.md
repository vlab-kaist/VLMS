---
share: "true"
title: Gradient Based Optimization
---
[Link](https://www.youtube.com/watch?v=atXrbIY6iyQ) for the video of Gradient Based Optimization.

### Introduction
##### What is optimization?
Optimization is selecting the best element with some criterion. Optimization problem is maximizing or minimizing functions by choosing inputs.[^1]

> [!Example] Real-life Optimizations Example
> - Optimizing the design to maximize the performance.
> - Optimizing the recommendation algorithm to show best personalized advertisement.
> - Optimizing the factory to spend less time and money.

### Mathematical Optimization
This is just finding $x$ that maximizes or minimizes some function $f(x)$. It is easy for some simple functions, i.e. quadratic functions.
$$
f(x)= ax^2 + bx+c \quad (a>0)
$$

To find $x$ that minimizes function $f(x)$, we simply differentiate $f(x)$.
$$
f'(x)=2ax+b=0
$$


<script type="text/tikz">
  \begin{tikzpicture}
    \draw (0,0) circle (1in);
  \end{tikzpicture}
</script>

---
[^1]: https://en.wikipedia.org/wiki/Mathematical_optimization