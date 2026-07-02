---
created:
tags:
  - math
subject:
  - Linear Algebra
---
# Core ideas
[[Interpolation]]

# Content
For a set of
$$x_{0} \dots,x_{n} \in \mathbb{K} \space \& \space y_{0} \dots,y_{n} \in \mathbb{K}$$
Newton suggests that:
$$
p(x) = A_{0} + A_{1}(x-x_{0}) + \dots + A_{n}(x-x_{n-1}) = \sum_{k=0}^n A_{k}\prod_{0≤j<k}(x-x_j)
$$
Where $A_0, \dots, A_n \in \mathbb{K}$ are unknown constants.
interpolates a function $f(x)$ that actually describes the dataset.

Example:
![[pdf24_merged.jpg]]
Importantly:
$$
\boxed{p(x)=A_0 + A_1(x-5,5)+A_2(x-5,5)(x-7,3)}
$$
is solvable, because it can be expressed as:
$$
\begin{gather}
A_0 = p(5,5) = f(5,5) \\ \\
A_1 = \frac{f(7,3) - A_0}{7,3-5,5} \\ \\
A_2 = \frac{f(10,2) - A_0 - A_1(10,2 - 5,5)}{(10,2-5,5)(10,2-7,3)} \\
\end{gather}
$$