[[Technote]] created on Th | 08-01-2026 18:20

# Core ideas

# Content
Bei einer linearen Abbildung ist es egal ob man zwei Vektoren zuerst addiert oder Abbildet
## Definition
Für $f:V\to W$ über Grundkörper $K$ muss gelten dass:
$$
\begin{gather}
additiv: \\
f(\vec{a}+\vec{b}) = f(\vec{a}) + f(\vec{b}) \\
homogen: \\
f(\vec{ax}) = xf(\vec{a}) \\
 \\
\vec{a},\vec{b} \in V \\
x \in K
\end{gather}
$$
> [!Important] Folgerung
>Eine Abbildung ist linear, wenn sie die Struktur des Vektorraumes nicht verändert.
>Somit ist jede [[Lineare Abbildung]] ein [[Homomorphismus]] über Vektorräume.
>Sie sind als [[Abbildungsmatrix]] darstellbar. Wobei die dimension der Räume die Form der Matrix bestimmt.
>$f:V\to W$ mit Dimensionen $dim(V)=n$ $dim(W)=m \implies m\times n$ [[Abbildungsmatrix]] $M_{W}^V(f)$
## Beispiel Aschenspiegelung als lineare Abbildung:
![[Pasted image 20260108182239.png]]
