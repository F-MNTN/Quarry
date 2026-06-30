[[Technote]] created on Th | 08-01-2026 15:40

# Core ideas
Abbildung durch eine [[Matrix]].
# Content
Nur für [[Endomorphismus]] berechenbar.
## General Concept
Ein [[EV - Eigenvektor]] einer Matrix $A$ ist ein Vektor $\neq \vec{0}$, dessen Richtung durch die Abbildung von $A$ nicht verändert wird.  Die EV werden also nur skaliert. Der [[EW - Eigenwert]] ist der Wert um den der [[EV - Eigenvektor]] skaliert wird. 
## Formale Definition
Für eine [[Matrix#Quadratische Matrix]] $A \in \mathbb{K}^{n \times n}$ heißt $\lambda \in \mathbb{K}$ [[EW - Eigenwert]], falls ein [[Vektor]] $\vec{v} \neq \vec{0}$ existiert mit:

## Wichtige Eigenschaften
### Spur:
$\sum_{i=1}^{n} \lambda_i = \operatorname{tr}(A)$ , siehe [[Matrix#Trace]] für Definition.
### Determinante: 
$\prod_{i=1}^n \lambda_i = \det(A)$
### Invertierbarkeit: 
$A$ invertierbar $\iff$ $0 \notin \sigma(A)$. Wobei $\sigma(A)$ die Menge der [[EW - Eigenwert]] von $A$ ist. Siehe [[Matrix#Invertierbar]] für weitere Kriterien

$$
\begin{gather}
A\vec{v} = \lambda\vec{v}
\end{gather}
$$
### Vielfachheit 
Wenn das [[Matrix#Charakteristisches Polynom]] als zb.: $(\lambda-1)(\lambda+1)(\lambda-4)$ darstellbar ist. Kann man einfach sehen, dass die EW $\{-1,1,4\}$ alle eine Vielfachheit von 1 haben.
Vgl.:
$(\lambda-5)^2*\lambda$ besitzt die EW $\{5,0\}$ wobei 5 in *zweifacher Vielfachheit* vorkommt.

>[!Note] Anmerkung
>Aus [[Matrix#Invertierbar]] wissen wir dass die Matrix bei einem $EW = 0$ nicht invertierbar sein kann.
## Berechnung
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
= -\lambda^3+4\lambda^2+\lambda-4 = (\lambda-1)(\lambda+1)(\lambda-4) \\ \\
(\lambda-1)(\lambda+1)(\lambda-4) = 0 \\
NST = EW = \lambda = \{1;-1;4\}
\end{gather}
$$
Wenn man jetzt aus irgendwelchen Gründen die $EW$ von $A^{-1}$ haben will kann man eine einfache Abkürzung nehmen und einfach den Kehrwert der $EW(A)$ berechnen.
$$
\begin{gather}
EW(A^{-1})_{i} = \frac{1}{EW(A)_{i}} & 1\leq i \leq dim(EW(A))
\end{gather}
$$
Von dem Punkt weg können die [[EV - Eigenvektor]] und [[ER - Eigenraum]] berechnet werden.

## Anwendungen
### Diagonalisierung:
Falls $A$ [[Matrix#Diagonalisierbar]], gilt $A = PDP^{-1}$ mit $D$ = Diagonalmatrix der EW. Wo $P$ die Abbildungsmatrix ist die von Eigenbasis zu Standardbasis abbildet.
$\implies P= M^{Eigenbasis}_{E}$ 
$\implies P^{-1}= M^{E}_{Eigenbasis}$
### Stabilitätsanalyse: 
In dynamischen Systemen geben [[EW - Eigenwert]] Auskunft über Stabilität
### Hauptachsentransformation:
In der Geometrie zur Bestimmung von Hauptachsen