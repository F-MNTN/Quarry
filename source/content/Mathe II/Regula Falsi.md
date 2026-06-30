[[Technote]] created on Tu | 20-01-2026 12:56

# Core ideas
[[Approximation]]
# Content
Ist ein Einschließungsverfahren, dass eine Nullstelle von $f(x)$ zwischen zwei Punkten $p_{1}(x_{n-1},f(a));p_{2}(x_{n-2},f(b))$ sucht. Wobei $sgn(f(x_{n-1})) = - sgn(f(x_{n-2}))$.

$$
\begin{gather}
x_{n} = x_{n-2} - \frac{x_{n-1}-x_{n-2}}{f(x_{n-1})-f(x_{n-2})}*f(x_{n-2}) \\
\end{gather}
$$