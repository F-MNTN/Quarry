---
created:
tags:
  - math
subject:
  - Linear Algebra
---
# Core ideas

Stellen oft [[Lineare Abbildung]] dar, wird dann [[Abbildungsmatrix]] genannt.

# Content

Geschrieben als:

$$
\begin{gather}
	A_{2,3} =
	\begin{bmatrix}
		a & b & c  \\
		d & e & f
	\end{bmatrix} \\
	A_{n,m} =
	\begin{bmatrix}
		x_{1,1} & x_{1,2} & \cdots & x_{1,m} \\
		x_{2,1} & x_{2,2} & \cdots & x_{2,m} \\
		\vdots  & \vdots  & \ddots & \vdots  \\
		x_{n,1} & x_{n,2} & \cdots & x_{n,m}
	\end{bmatrix}
\end{gather}
$$

## Einheitsmatrix

Gechrieben als $E_{n}$ oder $I_{n}$ ist eine [[Matrix#Quadratische Matrix]].
Sie hat den vollen Rang $n$.
Je nach [[Matrix#Dimension]] sieht sie so aus:

$$
E_{n} =
\begin{bmatrix}
1 & \dots & 0  \\
\vdots & \ddots_{1} & \vdots  \\
0 & \dots & 1
\end{bmatrix}
$$

Mit $1$ auf der Hauptdiagonale und sonst nur $0$.

## Nullmatrix

Eine [[Matrix]] von Dimension $n,m$ die nur mit 0 gefüllt ist.
Ist nicht unbedingt eine [[Matrix#Quadratische Matrix]].

$$
0_{n,m} =
\begin{bmatrix}
0 & \dots & 0  \\
\vdots & \ddots & \vdots  \\
0 & \dots & 0
\end{bmatrix}
$$

## Transponiert

Sei $A_{n,m} = \bigl[\begin{smallmatrix} a & b \\ c & d \end{smallmatrix} \bigr]$ eine Matrix, so ist $A^{T}_{m,n} = \bigl[\begin{smallmatrix} a & c \\ b & d \end{smallmatrix} \bigr]$ die transponierte Matix von A.
Es werden Zeilen und spalten vertauscht oder die Matrix an ihrer Hauptdiagonale gespiegelt.

## Invertierbar

Nur [[Matrix#Quadratische Matrix]] können invertiert werden. Die inverse Matrix ist definiert als $A * A^{-1} = A^{-1} * A = I$ Wobei $A$ eine [[Matrix#Regulär]] ist.

$$
\begin{gather}
A =
\begin{bmatrix}
2 & 1 \\
6 & 4
\end{bmatrix}
\iff A^{-1}=
\begin{bmatrix}
2 & -\frac{1}{2} \\
-3 & 1
\end{bmatrix}
 \\
A * A^{-1} =
\begin{bmatrix}
4-3 & -1+1 \\
12-12 & -3+4
\end{bmatrix}
=
\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}
= I \\
(cA)^{-1} = c^{-1}A^{-1} | c\neq 0 \in \mathbb{R} \\
(A^T)^{-1} = (A^{-1})^T \\
\det(A^{-1}) = \det(A)^{-1}
\end{gather}
$$

Eine Matrix ist invertierbar wenn:

- $\iff \det(A)\neq 0$
- $\iff$ alle [[EW - Eigenwert]] $\neq 0$
- $\implies$ sie vollen Rang hat $rang(A) =$ Anzahl von Reihen/Spalten von A
- $\iff x \mapsto Ax$ [[Bijektive Abbildung]] ist

## Diagonalisierbar

Eine [[Matrix#Quadratische Matrix]] $n \times n$-Matrix $A$ ist [[Matrix#Diagonalisierbar]] genau dann, wenn:

$$
\begin{gather} \\
\sum_{\lambda \in \sigma(A)} \dim(E_A(\lambda)) = n = dim(A)
\end{gather}
$$

wobei $\sigma(A)$ die Menge aller [[EW - Eigenwert]] von $A$ ist.

## Rang

Der Rang einer Matrix $rang(A) / rg(A)$ beschreibt die Anzahl der Zeilen die (zb mit dem [[Gaußschen Eliminationsverfahren]]) nicht auf 0-Zeilen reduziert werden können.

### Beispiel

$$
\begin{gather}
A =
\begin{bmatrix}
1 & 2 & 4 \\
0 & 5 & 4 \\
0 & 10 & 2
\end{bmatrix}
\to
\begin{bmatrix}
1 & 2 & 4 \\
0 & 5 & 4 \\
0 & 0 & -6
\end{bmatrix}
\implies rang(A) = 3
\\

B =
\begin{bmatrix}
1 & 2 & 4 \\
0 & 6 & 4 \\
0 & 3 & 2
\end{bmatrix}
\to
\begin{bmatrix}
1 & 2 & 4 \\
0 & 6 & 4 \\
0 & 0 & 0
\end{bmatrix}
\implies rang(B) = 2
\\
C =
\begin{bmatrix}
2 & 3 \\
0 & 1 \\
4 & -1
\end{bmatrix}
\to
\begin{bmatrix}
2 & 3 \\
0 & 1 \\
0 & 0
\end{bmatrix}
\implies rang(C) = 2
\end{gather}
$$

Alternativ gilt das gleiche bei Spaltenstufen für die Anzahl der Spalten die $\neq$ 0 sind

Wenn $rang(A)<dim(A)$ redet man von Dimensionsschwund.

## Dimension

$dim(A^{n*m}) = n*m$
Die dimensionale Ausbreitung einer Matrix. Simples Konzept mit wichtigen Zusammenhängen wie $dim(bild(A)) = rang(A)$.

## Kern

Ist die Lösungsmenge des [[Vektor]] $\vec{v}$ zu:

$$
\begin{gather}
A=
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
*
\begin{pmatrix}
v_{1} \\
v_{2}
\end{pmatrix}
= \vec{0} \\
\det(A) = 2 \neq 0 \iff ker(A) = \vec{0}
\end{gather}
$$

![[Pasted image 20260111154014.png]]
Wenn $\det(A) \neq 0$ ([[Matrix#Determinante]]) dann ist $A$ linear unabhängig und $ker(A)= \vec{0}$.
Bei $\det(A) = 0$ muss das Gleichungssystem von oben gelöst werden um $ker(A)=\vec{v}$ zu bekommen

### Beispiel

Matrix mittels [[Gaußschen Eliminationsverfahren]] in Zeilenstufenform (ZSF) bringen.

$$
\begin{gather} A=
\begin{bmatrix}
1 & 0 & -2 \\
3 & 1 & 0 \\
-1 & 0  & 2
\end{bmatrix} \to \dots \to
\begin{bmatrix}
1 & 0 & -2 \\
0 & 1 & 6 \\
0 & 0 & 0
\end{bmatrix}
\end{gather}
$$

Alle _0_ auf Hauptdiagonale als _1_ anschreiben und LGS lösen.

$$
\begin{gather} \\
\begin{bmatrix}
1 & 0 & -2 \\
0 & 1 & 6 \\
0 & 0 & 1
\end{bmatrix} =
\vec{0} \\
kern(A) = span\left\{
\begin{pmatrix}
2 \\
-6 \\
1
\end{pmatrix}
 \right\}
\end{gather}
$$

## Bild

Das Bild einer Matrix $M$ (oder einer [[Lineare Abbildung]] $f:V\to W$ die durch $M$ als [[Abbildungsmatrix]] dargestellt wird) ist die Menge aller $\vec{w} \in W$

$$
\begin{gather}
Bild(f) =\{\vec{w} \in W|\exists \vec{v} \in V : f(\vec{v})=\vec{w}\}
\end{gather}
$$

Und im Matrix-Fall:

$$
\begin{gather}
Bild(M) =\{y \in K^m|\exists x \in K^n : M*x=y\}
\end{gather}
$$

Für $f:V\to W$ gilt $Bild(f) \subseteq W$. Wenn $f$ [[Surjektive Abbildung]] sogar $Bild(f) = W$.
[[Vektor]] $\vec{w} \in W$ wird Bildvektor genannt.
Für alle Matrizen stimmt $dim(Bild(A)) = rang(A)$.

### Beispiel

$$
\begin{gather} A=
\begin{bmatrix}
1 & 3 & 2 \\
2 & 4 & 4 \\
3 & 5 & 6
\end{bmatrix} \\
bild(A)=A*\vec{v} = \vec{w} \\
\end{gather}
$$

Wobei man für $\vec{v}$ die kanonischen [[Vektor#Einheitsvektor]] einsetzt.

$$
\begin{gather}
A *
\begin{pmatrix}
1 \\
0 \\
0
\end{pmatrix} =
\begin{pmatrix}
1 \\
2 \\
3
\end{pmatrix} \\
A *
\begin{pmatrix}
0 \\
1 \\
0
\end{pmatrix} =
\begin{pmatrix}
3 \\
4 \\
5
\end{pmatrix}
 \\
A *
\begin{pmatrix}
0 \\
0 \\
1
\end{pmatrix} =
\begin{pmatrix}
2 \\
4 \\
6
\end{pmatrix} \\
\begin{pmatrix}
1 \\
2 \\
3
\end{pmatrix} * 2 =
\begin{pmatrix}
2 \\
4 \\
6
\end{pmatrix} \implies bild(A) = \langle
\begin{pmatrix}
1 \\
2 \\
3
\end{pmatrix},
\begin{pmatrix}
3 \\
4 \\
5
\end{pmatrix} \rangle  = \langle
\begin{pmatrix}
1 \\
2 \\
3
\end{pmatrix},
\begin{pmatrix}
0 \\
-1 \\
-2
\end{pmatrix} \rangle
\end{gather}
$$

## Determinante

Sagt aus um welchen Wert der Raum bei einer [[Lineare Abbildung]] skaliert sird.

$$
\begin{gather}
\det(A) =
\det\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 0
\end{bmatrix} =
1*5*0 + 2*6*7 + 3*4*8 - 7*5*3 - 2*4*0 - 1*6*8 = 27 \neq 0 \\

\det(B) =
\det\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{bmatrix} =
1*5*9 + 2*6*7 + 3*4*8 - 7*5*3 - 2*4*9 - 1*6*8 = 0
\end{gather}
$$

Da $A$ [[Matrix#Quadratische Matrix]] und $\det(A)\neq 0$ und somit [[Matrix#Invertierbar]] ist $A$ eine [[Matrix#Regulär]].
Wenn $\det(A)\neq 0$ dann ist das Gleichungssystem eindeutig lösbar ist. Nützlich bei [[Matrix#Kern]].

## Trace

Ist die Summe der Werte auf der Hauptdiagonale.

$$
\begin{gather}
tr(A)=\sum_{i=1}^{n}x_{ii} & n=dim(A)
\end{gather}
$$

Wichtig für [[EW - Eigenwert]].

## Eigenschaften einer Matrix

### Normal

Wenn $A*A^T = A^T*A$ ist eine Matrix $A$ normal. Vereinfacht einige Details. zB.: Orthogonalität der [[EV - Eigenvektor]]. Siehe [[ER - Eigenraum#$EV_{3} @ lambda = 3$]]!

### Symmetrisch

Wenn $A = A^T$

$$
\begin{gather}
A=
\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}=A^T
\end{gather}
$$

### Orthogonal

Wenn alle Vektoren $a_{i} \in A$ orthogonormal aufeinander sind. Orthogonal $\iff$[[Vektor#Vektormultiplikation (Dot Product)]]$=0$ und [[Vektor#Norm/Länge/Betrag]]$= 1$
$\implies A^T = A^{-1} \iff A^T*A = A^{-1}*A = I$
zb.:

$$
\begin{gather}
A=
\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}, A^{-1}=A^T=
\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix} \\
\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix} *
\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}
= I
\end{gather}
$$

### Regulär

[[Matrix#Quadratische Matrix]] die [[Matrix#Invertierbar]] ist.

### Singulär

[[Matrix#Quadratische Matrix]] die nicht [[Matrix#Invertierbar]] ist.

## Charakteristisches Polynom

Die Nullstellen dieses Polynoms ergibt alle [[EW - Eigenwert]] der Matrix.

$$
\begin{gather}A =
\begin{bmatrix}
1 & 0 & 1 \\
2 & 2 & 1 \\
4 & 2 & 1
\end{bmatrix} \\ \\
\chi_{A}(\lambda) = \det(A-\lambda*I_{3*3}) = \det
\begin{bmatrix}
1-\lambda  & 0 & 1 \\
2 & 2-\lambda & 1 \\
4 & 2 & 1-\lambda
\end{bmatrix} \\
= \lambda^3-4\lambda^2-\lambda+4 = (\lambda-1)(\lambda+1)(\lambda-4) \\ \\
NST = EW = \{1;-1;4\}
\end{gather}
$$

Also sind die [[EW - Eigenwert]] dieser Matrix $\left\{1,-1,4\right\}$.

## Definitheit

Hilft Aussagen über das Extremwertverhalten einer Matrix zu treffen.

### Sylvester/Hauptminoren-Methode

Sei $A$ eine [[Matrix#Quadratische Matrix]]. So sind die Hauptminoren die [[Matrix#Determinante]] der quadratischen Untermatrizen $\Delta_{i}$ entlang der Hauptdiagonale.

$$
\begin{gather}A_{n,n}=
\begin{bmatrix}
x_{11} & \dots & x_{n1} \\
\vdots & \ddots & \vdots \\
x_{n1} & \dots & x_{nn}
\end{bmatrix} \\
\Delta_{1} = \det
\begin{bmatrix}
x_{11}
\end{bmatrix} \\
\Delta_{2} = \det
\begin{bmatrix}
x_{11} & x_{12} \\
x_{21} & x_{22}
\end{bmatrix} \\
\Delta_{3} = \det
\begin{bmatrix}
x_{11} & x_{12} & x_{13} \\
x_{21} & x_{22} & x_{23} \\
x_{31} & x_{32} & x_{33}
\end{bmatrix} \\
\vdots \\
\Delta_{n} = \det(A)
\end{gather}
$$

Uns interessieren aber nur die Vorzeichen dieser Determinanten $\Delta_{i}$.

#### Positiv definit

Alle $\Delta_{i}$ sind positiv. $\{+,+,+,+,+,+,\dots\}$
Dies weist auf ein _Minimum_ hin.

#### Positiv semidefinit

So wie [[Matrix#Positiv definit]] aber manchmal kommt $0$ vor

- $\{+,0,+,0,0,+,+,\dots\}$
  Geometrisch weißt das entweder auf einen _Sattelpunkt oder ein Minimum_ (Maximum kann ausgeschlossen werden)

#### Indefinit

Jeder Fall der nicht mit zu den anderen passt.
Geometrisch weißt das auf einen _Sattelpunkt_

#### Negativ semidefinit

So wie [[Matrix#Negativ definit]] aber manchmal kommt $0$ vor

- $\{-,0,-,0,0,+,-,\dots\}$
  Es gilt:
- $\Delta_{i}\geq0$ wo $i\%2=0$
- $\Delta_{i}\leq0$ wo $i\%2=1$
  Geometrisch weißt das entweder auf einen _Sattelpunkt oder ein Maximum_ (Minimum kann ausgeschlossen werden)

#### Negativ definit

Wenn sich die Reihenfolge $\{-,+,-,+,-,+,-,+,\dots\}$ ist, also:

- $\Delta_{i}>0$ wo $i\%2=0$
- $\Delta_{i}<0$ wo $i\%2=1$
  Geometrisch weißt das auf ein _Maximum_ hin.

### Anhand Eigenwerten

Wenn alle [[EW - Eigenwert]] in eines der Muster in der Tabelle passen folgt:

| _EW_    | _Definitheit_    | _Geometrisch_        |
| ------- | ---------------- | -------------------- |
| >0      | pos. Definit     | Minimum              |
| ≥0      | pos. Semidefinit | Min oder Sattelpunkt |
| <0      | neg. Definit     | Maximum              |
| ≤0      | neg. Semidefinit | Max oder Sattelpunkt |
| - und + | Indefinit        | Sattelpunkt          |

## Quadratische Matrix

Sind Matrizen wo $M_{n,m}|n=m$.
Wenn [[Matrix#Invertierbar]] dann [[Matrix#Regulär]] sonst [[Matrix#Singulär]].
Kann als [[Abbildungsmatrix]] eine [[Bijektive Abbildung]] beschreiben wenn:

- $det(A) \neq 0$
- $rang(A) = n$
- $ker(A) = \{0\}$
- $0$ kein [[EW - Eigenwert]] ist

## Drehmatrix

Rotiert einen Vektor um den Winkel $\alpha$ um den Ursprung.

$$
\begin{gather}
R_{\alpha}=
\begin{bmatrix}
\cos \alpha & -\sin \alpha \\
\sin \alpha & \cos \alpha
\end{bmatrix}
\end{gather}
$$

## Spiegelmatrix

Sei $g$ eine Gerade durch den Ursprung mit Neigungswinkel $\alpha$ an der gespiegelt wird.

$$
\begin{gather}
S_{g} =
\begin{bmatrix}
\cos 2\alpha & \sin 2 \alpha \\
\sin 2 \alpha & -\cos 2 \alpha
\end{bmatrix}
\end{gather}
$$

## Operationen von Matrizen

### Matrixaddition

Die Matrizen werden elementweise addiert.

$$
\begin{gather}
\begin{bmatrix}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{bmatrix} +
\begin{bmatrix}
b_{11} & b_{12} \\
b_{21} & b_{22}
\end{bmatrix} =
\begin{bmatrix}
a_{11} + b_{11} & a_{12} + b_{12} \\
a_{21} + b_{21} & a_{22} + b_{22}
\end{bmatrix}
\end{gather}
$$

#### Kompatibilitätskriterien

Die Matrizen $A,B$ müssen von gleichen Dimensionen sein.

### [Matrixmultiplikation](https://de.wikipedia.org/wiki/Matrizenmultiplikation)

Komponentenweise Verknüpfung zweier Matrizen. $A_{n,m} * B_{d,f} = C_{n,f}$

$$
\begin{gather}
A * B =
\begin{bmatrix}
0 & 4 & -2 \\
-4 & -3 & 0
\end{bmatrix} *
\begin{bmatrix}
0 & 1 \\
1 & -1 \\
2 & 3
\end{bmatrix}
=
\begin{bmatrix}
0 * 0 + 4 * 1 - 2 * 2 & 0 * 1 - 4 * 1 - 2 * 3 \\
-4 * 0 - 3 * 1 + 0 * 2 & -4 * 1 + 3 * 1 + 0 * 3
\end{bmatrix}
=
\begin{bmatrix}
0 & -10 \\
-3 & -1
\end{bmatrix} = C_{n,f}
\end{gather}
$$

#### Kompatibilitätskriterien

Damit eine Matrixmultiplikation stattfinden kann, muss $m$ (Anzahl der Spalten von $A$) $= d$ (Anzahl der Zeilen von $B$) sein.

### Matrix-Vektor Produkt

Wir sehen [[Vektor]] als Spaltenmatrix an.

$$
\begin{gather}
M_{2,3} * \vec{v} =
\begin{bmatrix}
1 & -1 & 2 \\
0 & -3 & 1
\end{bmatrix}
*
\begin{bmatrix}
2 \\
1 \\
0
\end{bmatrix}
=
\begin{bmatrix}
2 * 1 - 1 * 1 + 0 * 2 \\
2 * 0 - 1 * 3 + 0 * 1
\end{bmatrix}
=
\begin{bmatrix}
1 \\
-3
\end{bmatrix}
= W_{2,1}
\end{gather}
$$

#### Kompatibilitätskriterien

Bei einem Produkt $M_{n,m} * \vec{v}$ muss die Anzahl der Zeilen des [[Vektor]] $dim(\vec{v}) = d$ gleich der Anzahl der Spalten $m$ der Matrix sein damit die Operation möglich ist.
Die resultierende Matrix ist dann von Dimension $W_{n,1}$

# Relevant Links

[[Vektor#Kreuzprodukt]] nicht hier zu finden aber trotzdem relevant.

