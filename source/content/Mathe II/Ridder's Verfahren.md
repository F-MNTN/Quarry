[[Technote]] created on Tu | 20-01-2026 12:54

# Core ideas

# Content
Ist eine Verbesserung von [[Regula Falsi]] durch superlineare Konvergenz.
$$
\begin{gather}
& a<b &  f(a)*f(b)<0 \\
d=\frac{b-a}{2} & m=\frac{a+b}{2}   \iff &  m=a+d  & b=a+2d
\end{gather}
$$
## Schritt 1:
Wähle q $\in \mathbb{R}$ dass $h(x):= e^{qx}*f(x)$ erfüllt $h(m)=\frac{h(a)+h(b)}{2}$.
## Schritt 2:
Berechne Nullstelle $c$ der Sekante durch $(m,h(m))$ and $b,h(b)$.
$$
\begin{gather}
\text{Bsp für: }P_{1}(1,3),P_{2}(5,5) \\
S(x)=\frac{h(m)-h(b)}{m-b}x+d \\
\text{Dann setzt man einen Punkt der definitiv auf der Geraden ist ein zb $P_{1}(1,3)$} \\
3=\frac{2}{4}*1+d\\
d=\frac{5}{2}
\end{gather}
$$
## Schritt 3:
Neues Intervall wählen mit Grenzen $c,\dot{c}$ , wo $\dot{c} \in \{a,m,b\}, f(c)*f(\dot{c})<0$ und $|c-\dot{c}|$ kürzestmöglich. 