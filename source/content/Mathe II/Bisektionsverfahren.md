[[Technote]] created on Tu | 20-01-2026 14:22

# Core ideas
[[Approximation]]
# Content
Ist ein Einschließungsverfahren (wie [[Regula Falsi]]) und kann für Nullstellen verwendet werden.
Wobei man eine Nullstelle zwischen 2 Punkten $p(x_{n-1},f(x_{n-1})),p(x_{n-1},f(x_{n-1}))$ sucht mit $sgn(f(x_{n-1})) = - sgn(f(x_{n-2}))$.
Prozess:
$$
\begin{gather}
m_{1} = \frac{a+b}{2}
\end{gather}
$$

Je nachdem ob $f(m)>0$ oder $f(m)<0$ wird entweder $a=m_{2}$ oder $b=m_{2}$ gesetzt für die nächste Iteration, sodass $f(a)*f(b)<0$. Dies wird wiederholt bis die gewünschte $\epsilon$-Umgebung erreicht ist.