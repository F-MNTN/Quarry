---
created:
tags:
  - math
subject:
  - Linear Algebra
---
# Core ideas
[[Morphismus]]
Mathematische Struktur
# Content
Ist eine algebraische Abbildung bei der die mathematische Struktur erhalten bleibt.
## Example
### Gruppenhomomorphismus
Seien $(\mathbf{A},\star) , (B, \bullet)$ Gruppen mit Operationen $\star, \bullet$ respektiv.
Der Gruppen-Homomorphismus $f: A\to B$ besagt, dass 
$$
\begin{gather}
f(x \star y) = f(x)\bullet f(y) \\
f(e_{A}) = e_{B} \\
f(x^{-1}) = f(x)^{-1} \\
x,y \in A
\end{gather}
$$

### Ringhomomorphismus
Seien $R,S$ Ringe mit Operationen $+,*$
Dann ist $f$ eine Funktion, dass:
$$
\begin{gather}
I: f(a+b) = f(a) + f(b) \\
II:_{ }f(a*b) = f(a) * f(b) \\
a,b \in \mathbb{R} \\
III: f(e_{R}) = e_{S}
\end{gather}
$$

### Video Example
[Gruppenhomomorphismus, Definition und Beispiel | Mathe by Daniel Jung​](https://www.youtube.com/watch?v=NXjtsxTRtYE)

### Implications
Eine [[Bijektive Abbildung]] die auch ein [[Homomorphismus]] ist heißt [[Isomorphismus]].