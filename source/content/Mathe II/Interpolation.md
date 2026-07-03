---
created:
tags:
  - math
subject:
  - Linear Algebra
---
# Core ideas
Interpolation is a method to smooth functions. Depending on the size of a dataset it may perform better/worse than [[Approximation]].
# Content

## Kinds of Interpolation

### Polynomial Interpolation
Let $f_n:  \mathbb{K} → \mathbb{K} \space x→x^n$ be a Monom function for $n \in \mathbb{N}$

Ansatz: 
$$
\begin{gather}
\phi_{n}(a_{0}, \dots, a_{n}, f_{0},\dots, f_{n}) = a_{0}f_{0} + \dots + a_{n}f_{n}\\
\implies \phi(\dots) = a_{0}x^0+\dots+a_{n}x^n \\
\end{gather}
$$
for $x \in \mathbb{K}$
### Trigonometric Interpolation
Let $f_{n}: \mathbb{C} \to \mathbb{C} \space z \to \exp(i*n*z)$
Ansatz:
$$
\begin{gather} \\
\phi_{n}(a_{0}, \dots, a_{n}, f_{0},\dots, f_{n}) = a_{0}f_{0} + \dots + a_{n}f_{n}\\
\implies \phi(\dots)(z) = a_{0}\exp(i*z)^0+\dots+a_{n}\exp(i*z)^n \\
\end{gather}
$$
for $z \in \mathbb{C}$

# References
[Polynominterpolation – Wikipedia](https://de.wikipedia.org/wiki/Polynominterpolation)
- [Lagrange polynomial - Wikipedia](https://en.wikipedia.org/wiki/Lagrange_polynomial)
- [Polynominterpolation | Newton Basis – Wikipedia](https://de.wikipedia.org/wiki/Polynominterpolation#Ansatz:_Newton-Basis)
	- [[Mathe_II_Skriptum.pdf#page=12|Mathe_II_Skriptum, p.12]]