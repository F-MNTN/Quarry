---
created: 2026-06-22
tags:
  - Chemistry
subject:
  - Analytical Chemistry
  - Basics
---
# Core ideas
[[Säure-Base]] Verhalten
[[pH-Wert]] einer Lösung bestimmen und vorhersagen
# Content
Ausgehend von einem gelösten Stoff und seiner Konzentration, können schnell Aussagen über das [[Säure-Base]] Verhalten der Lösung gemacht werden.

## Protolyse von Salzen
Wenn ein Salz vorliegt als lösende Substanz, dann wird diese zuerst in einem Protolyseschritt in die jeweiligen Ionen aufgetrennt.
$$
\begin{gather}
\ce{NaAc -> Na+ + Ac- }
\end{gather}
$$
In diesem Fall wäre $Ac$ dann für die weitere Dissoziation der Ausgangsstoff.
## Protonenbilanzgleichung (PBA)
$$
\begin{gather}
\ce{HAc + H2O \leftrightarrow H3O+ + Ac- } \\
\ce{2H2O \leftrightarrow H3O+ + OH- } \\
 \\
\Sigma: \ce{H3O+ = OH- + Ac- }
\end{gather}
$$
Diese lässt sich vereinfachen auf die Dominanten Spezien der jeweiligen Seite
$$
\begin{gather}
\Sigma: \ce{H3O+ = Ac- }
\end{gather}
$$
Wobei dieser Schnittpunkt unsere Approximation für den pH wert im Diagramm ablesen lässt.
### Schnittpunktmatrix
|log c|$OH^-$|$Ac^-$|
| --- | --- | --- |
|$H^+$|  …   | … |
Die Schnittpunktmatrix besteht auf den Seiten aus den Elementen der PBA. Die Größen (hier "…") sind die $log(c)$ Werte die aus dem Diagramm gelesen werden. Hierbei gilt der Schnittpunkt der vereinfachten PBA wiederrum als der [[pH-Wert]] der Lösung.

## Gerechneter pH-Wert
Der pH Wert kann wie folgt errechnet werden:
$$
\begin{gather}
pH = \frac{pKs - \log(c)}{2}
\end{gather}
$$
bzw. für Salze mehrprotoniger Säuren/Basen gilt (zB.: $\ce{NaHS}$):
$$
\begin{gather}
pH = \frac{pKs_{1}+pKs_{2}}{2}
\end{gather}
$$
als Näherung.

![[Pasted image 20260622193223.png]]