---
created:
tags:
  - math
subject:
  - Linear Algebra
---
# Core ideas
[[EW - Eigenwert]]
[[Matrix]]
[[Lineare Abbildung]]
# Content
## Formale Definition
Ein EV $\vec{v}$ erfüllt:
$$
\begin{gather}
A*\vec{v} = \lambda * \vec{v} \\
\text{Für EW } \lambda \\
\vec{v} \neq \vec{0}
\end{gather}
$$
Für eine [[Lineare Abbildung]] $f:V\to W$, die durch die [[Abbildungsmatrix]] $A$ beschrieben wird sind [[EV - Eigenvektor]] die Vektoren die nur gestreckt/gestaucht werden. Die Richtung ist bei dieser Operation invariant.
## Berechnung
Durch lösen nach $\vec{v}$ von:
$$
\begin{gather}
(A-\lambda*I) *\vec{v} = \vec{0}
\end{gather}
$$
Erhält man den [[ER - Eigenraum]] zu dem eingesetzen [[EW - Eigenwert]] $\lambda$. Dies sollte für alle [[EW - Eigenwert]] wiederholt werden.
$$
\begin{gather}
ER_{A} = \left\{
t_{1}*
\vec{v_{1}},\dots ,
t_{n}*
\vec{v_{n}},
t_{i} \in \mathbb{R}
\right\} \\
\text{Wo } \vec{v_{i}} \text{ die EV von A.}
\end{gather}
$$

## Zusammenhang EV & ER
Der [[ER - Eigenraum]] besteht aus der Menge aller [[EV - Eigenvektor]] zu einem spezifischen [[EW - Eigenwert]]. Siehe [[ER - Eigenraum#Berechnung]]. Die [[EV - Eigenvektor]] (Anzahl je nach $dim(ER)$ siehe [[EW - Eigenwert#Vielfachheit]]) zu einem spezifischen [[EW - Eigenwert]] sind [[Vektorraum#Basis]] des aufgespannten  [[ER - Eigenraum]].