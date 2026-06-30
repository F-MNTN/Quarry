[[Technote]] created on Fr | 09-01-2026 15:58

# Core ideas

# Content
Vektoren sind mathematische Objekte, die aus Länge und Richtung bestehen. Als solches sind sie frei von einem bestimmten Punkt sondern können verwendet werden um zb eine gewisse Änderung einer Größe an einem Punkt darzustellen.
Siehe [[Faradaysches Gesetz]] oder [[Herz´sche Dipole]]

Insofern werden Vektoren nur als Änderungen in diversen Dimensionen angeschrieben: $\vec{v}=\bigl( \begin{smallmatrix}x \\ y\end{smallmatrix}\bigr)$ 
## Addition
Vektoren werden Elementenweise addiert
## Multiplikation
### Skalarmultiplikation
Ein Skalar skaliert den gesamten Vektor und wird somit in alle Dimensionen eingerechnet
$$
\begin{gather}
x * 
\begin{pmatrix}
a \\
b \\
c
\end{pmatrix} =
\begin{pmatrix}
xa \\
xb \\
xc
\end{pmatrix}
\end{gather}
$$
### Vektormultiplikation (Dot Product)
Vektoren werden elementweise Multipliziert und diese Werte werden danach addiert.
$$
\begin{gather}
\begin{pmatrix}
a \\
b \\
c
\end{pmatrix}*
\begin{pmatrix}
d \\
e \\
f
\end{pmatrix} =
a*d + b*e + c*f
\end{gather}
$$
> [!Note] [Skalarprodukt = 0](https://de.wikipedia.org/wiki/Skalarprodukt#Beispiele)
> Wenn das Skalarprodukt zweier Vektoren = 0 ist, dann sind sie aufeinander orthogonal(normal)
## Kreuzprodukt
$$
\begin{gather}
\vec{a}\times\vec{b} = 
\begin{pmatrix}
4 \\
2 \\
-5
\end{pmatrix}
\times
\begin{pmatrix}
0 \\
4 \\
6
\end{pmatrix}
= 
\begin{pmatrix}
2*6-4*(-5) \\
-5*0 - 6*4 \\
4*4-2*0
\end{pmatrix}
=
\begin{pmatrix}
32 \\
-24 \\
16
\end{pmatrix}
\end{gather}
$$
Das Ergebnis des Kreuzprodukts ist ein Vektor, der Normal zu den beiden ist die in der Operation teilgenommen haben. 
![[Cross_product_parallelogram.gif]]
>[!Important] Kreuzprodukt = 0
>Dann ist die von ihnen aufgespannte Fläche = 0 $\implies$ sie sind Skalierungen voneinander.
### Kompatibilitätskriterien
Die zwei Vektoren $\vec{a} \times \vec{b}$ müssen von gleicher dimension sein.

## Norm/Länge/Betrag
Die Norm eines Vektors ist seine geometrische Länge.
Definiert als die Wurzel der Summe der Quadrate seiner Ausbreitungen. Grüße an Pythagoras.
$$
\begin{gather}
|\vec{a}|=\sqrt{\sum_{i = 1}^n{a_{i}}^2} \\
n = dim(a)
\end{gather}
$$
## Winkel zwischen Vektoren
Ist definiert als:
$$
\begin{gather}
\cos(\phi) = \frac{\vec{a}*\vec{b}}{|\vec{a}|*|\vec{b}|}
\end{gather}
$$

## Normierter Vektor
SInd vektoren dessen Länge 1 beträgt also $\hat{a} = \frac{\vec{a}}{|\vec{a}|}$.

## Einheitsvektor
Sind die [[Vektor#Normierter Vektor]] die im Koordinatensystem nur in eine Richtung Ausbreitung haben.
$$
\begin{gather}
\mathbb{R}^3: \\
\begin{pmatrix}
1 \\
0 \\
0
\end{pmatrix},
\begin{pmatrix}
0 \\
1 \\
0
\end{pmatrix},
\begin{pmatrix}
0 \\
0 \\
1
\end{pmatrix}
\end{gather}
$$