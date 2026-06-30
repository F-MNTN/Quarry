[[Technote]] created on Tu | 20-01-2026 12:22

# Core ideas
[[Interpolation]]

# Content
Given a set of $n$ coordinates  Lagrange Interpolation creates a polynomial $p(x)$ of degree $n-1$.

For a set of:
$$
\begin{gather}
x_{0} \dots,x_{n} \in \mathbb{K} \space \& \space y_{0} \dots,y_{n} \in \mathbb{K} 
\\
0 ≤ k ≤ n: p_{k} : \mathbb{K} →  \mathbb{K}
\end{gather}
$$
thus:
$$
\begin{gather}
p_{k} (x)= \frac{ (x−x_{0})(x−x_{1})...(x−x_{k-1})(x−x_{k+1})...(x−x_{n})}{
(x_{k}−x_{0})(x_{k}−x_{1})...(x_{k}−x_{k-1})(x_{k}−x_{k+1})...(x_{k}−x_{n})}   \\ \\
p(x)=\sum_{k=0}^{n} y_{k}p_{k}(x)
\end{gather}
$$
![[Pasted image 20251109233632.png]]

So for this example:
![[99 - Meta/Attachments/Mathe_II_Skriptum 2.jpg]]
referring to above:
$p(x) = f(x_{0})p_{0}(x) + f(x_{1})p_{1}(x) + f(x_{2})p_{2}(x)$


Results:
$$
p(x) = 630*\frac{(x-7,3)(x-10,2)}{(5,5-7,3)(5,5-10,2)}+900*\frac{(x-5,5)(x-10,2)}{(7,3-5,5)(7,3-10,2)}+1090*\frac{(x-5,5)(x-7,3)}{(10,2-5,5)(10,2-7,3)}
$$
$$
\boxed{p(x)=-17,975x^2 + 380,081x - 916,698}
$$
