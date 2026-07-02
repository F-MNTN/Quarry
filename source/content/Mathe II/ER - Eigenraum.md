---
created:
tags:
  - math
subject:
  - Linear Algebra
---
# Core ideas
[[EW - Eigenwert]]
[[EV - Eigenvektor]]
# Content
Ist die Menge aller [[EV - Eigenvektor]] zu einem [[EW - Eigenwert]].

## Berechnung
$$
\begin{gather}
A=
\begin{bmatrix}
1  & 2  &  -1 \\
0 &  3 &  0 \\
-1 &  2 &  1
\end{bmatrix} \\
\det(A-\lambda I) = 0 \\
\det
\begin{bmatrix}
1-\lambda  & 2  &  -1 \\
0 &  3-\lambda &  0 \\
-1 &  2 &  1-\lambda
\end{bmatrix} =
(1-\lambda)^2*(3-\lambda) +0+0 - (3-\lambda)-0-0 = (1-\lambda)^2*(3-\lambda) - (3-\lambda) \\
\dots \\
EW(A) = \{0,2,3\}
\end{gather}
$$
Um die [[EV - Eigenvektor]] zu bekommen setzt man nun die [[EW - Eigenwert]] als $\lambda$ in $(A-\lambda*I)*\vec{x}=0$ ein und löst das LGS.
### $EV_{1} @ \lambda = 0$
$$
\begin{align}
\begin{bmatrix}
 1 & 2 & -1 \\
0 & 3 & 0 \\
-1 & 2 & 1
\end{bmatrix} * \vec{x} = \vec{0} \\
x_{1}+2x_{2}-x_{3}=0  &  & I\\
3x_{2}=0  &  & II\\
-x_{1}+2x_{2}+x_{3}=0  &  & III\\ \\

\implies x_{2}=0  &  & II\\
\implies x_{1}=x_{3}  &  & I\&III\\
\end{align}
$$
$$
\begin{gather}
EV(A)_{\lambda=0} = 
\left\{
t *
\begin{pmatrix}
1 \\
0 \\
1
\end{pmatrix}
, t \in \mathbb{R}
\right\}
\end{gather}
$$
Diese Menge heißt Eigenraum von dem [[EW - Eigenwert]]. Da es einen Wert in dem Raum gibt ist $dim(EV(A)_{\lambda=0})=1$
### $EV_{2} @ \lambda = 2$
$$
\begin{align}
\begin{bmatrix}
 -1 & 2 & -1 \\
0 & 1 & 0 \\
-1 & 2 & -1
\end{bmatrix} * \vec{x} = \vec{0} \\
-x_{1}+2x_{2}-x_{3}=0  &  & I\\
x_{2}=0  &  & II\\
-x_{1}+2x_{2}-x_{3}=0  &   & III\\ \\

\implies x_{2}=0  &  & II\\
\implies -x_{1}=x_{3}  &  & I\&III\\
\end{align}
$$
$$
\begin{gather}
EV(A)_{\lambda=2} = 
\left\{
t *
\begin{pmatrix}
-1 \\
0 \\
1
\end{pmatrix}
, t \in \mathbb{R}
\right\} \\
dim(EV(A)_{\lambda=2})=1
\end{gather}
$$
### $EV_{3} @ \lambda = 3$
Da A *nicht normal* kann der letzte [[EV - Eigenvektor]] nicht über [[Vektor#Kreuzprodukt]] berechnet werden, obwohl es keine [[EW - Eigenwert#Vielfachheit]] >1 gibt.
Bei *normalen* Matrizen gilt im Allgemeinen, dass die [[EV - Eigenvektor]] zu verschiedenen [[EW - Eigenwert]] orthogonal sind. Bei *nicht normalen* Matrizen kann man so ein Aussage nicht treffen.
$$
\begin{align}
\begin{bmatrix}
 -2 & 2 & -1 \\
0 & 0 & 0 \\
-1 & 2 & -2
\end{bmatrix} * \vec{x} = \vec{0} \\
-2x_{1}+2x_{2}-x_{3}=0  &  & I\\
0=0 &  & II \\
-x_{1}+2x_{2}-2x_{3}=0  &  & III\\  \\


x_{3} = -2x_{1}+2x_{2} &  & I \\
x_{1}=2x_{2}+4x_{1}-4x_{2}  &  & III \\
-3x_{1}=-2x_{2} \\
x_{1} = \frac{2}{3}x_{2} \\
x_{2}=3 &  & setzen \\
\implies x_{1} = 2  &  &  III\\
\implies x_{3}=2 &  & I
\end{align}
$$
$$
\begin{gather}
EV(A)_{\lambda=3} = 
\left\{
t *
\begin{pmatrix}
2 \\
3 \\
2
\end{pmatrix}
, t \in \mathbb{R}
\right\} \\
dim(EV(A)_{\lambda=3})=1
\end{gather}
$$
Alle [[ER - Eigenraum]] von A sind 1-dimensional, da keiner der [[EW - Eigenwert]] eine Vielfachheit $>1$ hat
$$
\begin{align}
E_A(0) = \operatorname{span}\left\{\begin{pmatrix}1\\0\\1\end{pmatrix}\right\} \\
E_A(2) = \operatorname{span}\left\{\begin{pmatrix}-1\\0\\1\end{pmatrix}\right\} \\ 
E_A(3) = \operatorname{span}\left\{\begin{pmatrix}2\\3\\2\end{pmatrix}\right\}
\end{align}
$$

## Formale Definition
Für eine quadratische Matrix $A \in \mathbb{K}^{n, n}$ und einen Eigenwert $\lambda$ ist der **Eigenraum** definiert als:
$$
\begin{gather}
E_A(\lambda) = \{ v \in \mathbb{K}^n \mid A v = \lambda v \} = \ker(A - \lambda I_n)
\end{gather}
$$
Der Eigenraum ist immer ein **Untervektorraum** von $\mathbb{K}^n$ und enthält den Nullvektor $\vec{0}$.

## Vielfachheit
### Algebraische Vielfachheit:
Anzahl der Wiederholungen von $\lambda$ als Nullstelle im charakteristischen Polynom $\det(A - \lambda I)$
### Geometrische Vielfachheit: 
$\dim(E_A(\lambda)) = \dim(\ker(A - \lambda I))$

Es gilt im Allgemeinen: $\text{geom. Vielf.} \leq \text{alg. Vielf.}$
Im Beispiel: Alle Eigenwerte haben algebraische und geometrische Vielfachheit 1, also ist $A$ [[Matrix#Diagonalisierbar]].
