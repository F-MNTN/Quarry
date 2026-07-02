---
created:
tags:
  - math
subject:
  - Linear Algebra
---
[[Matrix]]
[[Lineare Abbildung]]
[[Injektive Abbildung]]
[[Surjektive Abbildung]]
[[Bijektive Abbildung]]
# Content
Beschreibt eine [[Lineare Abbildung]] zwischen zwei endlich-dimensionalen Vektorräumen.
Für die Funktion $f:V\to W$ ist die [[Abbildungsmatrix]] geschrieben als $M_{B}^A(f) * \vec{x}= \vec{y}$ wo $\vec{x}$ ein Vektor ausgedrückt in Basis $A=\left\{a_{1},a_{2},\dots,a_{n}\right\}$ ist der auf $\vec{y}$ in Basis $B=\left\{b_{1},b_{2},\dots,b_{m}\right\}$ abgebildet wird.

Diese Matrix $M_{B}^A(f)$ bildet die Vektoren aus Basis $A$ in Basis $B$ ab. 
$\implies$ Für jeden Basisvektor $a_{i}$ in $A$ gibt es einen Bildvektor (Ref.: [[Matrix#Bild]]) $f(a_{i})$ der sich als Linearkombination der Basisvektoren von $B$ darstellen lässt.
## Basiswechsel
$$
\begin{gather}
f:\mathbb{R}^2\to \mathbb{R}^2 \\
\begin{pmatrix}
x \\
y
\end{pmatrix}\mapsto
\begin{bmatrix}
12x+3y \\
-2x+7y
\end{bmatrix}
\end{gather}
$$
In Standardbasis $I_{2} = \bigl[\begin{smallmatrix} 1 & 0 \\ 0 & 1 \end{smallmatrix} \bigr]$ kann man schreiben $f = \bigl[\begin{smallmatrix} 12 & 3 \\ -2 & 7 \end{smallmatrix} \bigr]$. Wenn man jetzt aber Vektoren aus einer anderen Basis $B$ mit $f()$ verknüpfen will, geht man folgend vor:
$$
\begin{gather}
M^E_{E}(f) =
\begin{bmatrix}
12 & 3 \\
-2 & 7
\end{bmatrix} \\
B = \left\{
\begin{pmatrix}
1 \\
2
\end{pmatrix},
\begin{pmatrix}
2 \\
12
\end{pmatrix}
\right\} \to M^{B}_{E}=
\begin{bmatrix}
1 & 2 \\
2 & 12
\end{bmatrix} \\
M^{B}_{E}*\vec{v}_{B} = \vec{v}_{E}
\end{gather}
$$
$M^B_{E}$ ist somit die Abbildungsmatrix die von Basis $B$ in Standardbasis $E$ abbildet.
$$
\begin{gather}
{M^{B}_{E}}^{-1}*M^E_{E}(f)*M^{B}_{E} = M^B_{B}(f) \\
\end{gather}
$$
$M^{B}_{E_{2}}$ muss invertiert werden.
$$
\begin{gather} \\
{M^{B}_{E}}^{-1}= 
\begin{bmatrix}
\frac{3}{2} & -\frac{1}{4} \\
-\frac{1}{4} & \frac{1}{8}
\end{bmatrix} \\
M^{B}_{B}(f) = {M^{B}_{E}}^{-1}*M^E_{E}(f)*M^{B}_{E} \\
M^{B}_{B}(f) = 
\begin{bmatrix}
22 & 61 \\
-3 & -\frac{13}{2}
\end{bmatrix}
\end{gather}
$$
Wo $M^B_{B}(f)$ die Matrix ist die für Basis $B$ in Standardbasis $E$ transformiert, dann $f$ anwendet und wieder von $E$ zu $B$ transformiert.