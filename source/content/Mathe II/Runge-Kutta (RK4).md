---
created:
tags:
  - math
subject:
  - Linear Algebra
---
# Core ideas
[[Approximation]]
[[Differentialgleichung]]

# Content
Für eine [[Differentialgleichung#1. Ordnung]] $\frac{dy}{dx} = f(x,y)$ mit Anfangsbedingung $y(x_{0}) = y_{0}$ berechnet man Näherungswerte $y_{n} \approx y(x_{0}+nh), n=1,2,3,\dots$
Mit Verfahren wie folgt:
Ausgehend von:
$$
\begin{gather}
x_{n-1} = x_{0}+(n-1)h \\
y_{n-1} 
\end{gather}
$$
dabei definiert man $h$ als die gewollte Schrittlänge. 
## RK4
$$
\begin{gather}
k_{1}=hf(x_{n-1},y_{n-1})\\
k_{2}=hf\left( x_{n-1}+\frac{h}{2},y_{n-1}+\frac{k_{1}}{2} \right) \\
k_{3}=hf\left( x_{n-1}+\frac{h}{2},y_{n-1}+\frac{k_{2}}{2} \right) \\
k_{4}=hf\left( x_{n-1}+\frac{h}{2},y_{n-1}+k_{3} \right) \\
 \\
y_{n} = y_{n-1} + \frac{1}{6}(k_{1}+2k_{2}+2k_{3}+k_{4})
\end{gather}
$$
Das ist eine Iteration, bei weiteren Iterationen wird $y_{n}\text{ das neue }y_{n-1}$.