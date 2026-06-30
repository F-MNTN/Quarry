---
created: 2026-06-26
tags:
  - Chemistry
subject:
  - Analytical Chemistry
  - Basics
---
# Core ideas
Statistische Tests existieren um die Qualität der gesammelten Daten zu beurteilen, vergleichen und bereinigen zu können.
# Content
Je nach Fragestellung führt ein anderer Test zum gewollten Ergebnis.
![[Pasted image 20260626165328.png]]
## Grubbs' Ausreißer-Test
Grubbs schaut sich die Abstände der Werte zum Mittel im Verhältnis zur Standardabweichung an.
![[Pasted image 20260626165435.png]]
Es wird dann wie folgt gerechnet:
$$
\begin{align}
PW  & = \frac{|x_{i}-\bar{x}|}{\sigma} \\
PW  & > rM(f,95\%) \to \text{Ausreißer} \\
PW  & \leq rM(f,95\%) \to \text{kein Ausreißer} \\
f  & = n \text{(Anzahl der Messwerte)}
\end{align}
$$
### Beispiel
![[Pasted image 20260626165817.png]]
Wobei die Ergebnise von $rM(f, 95\%)$ aus einer Tabelle ausgelesen werden können.
## Student-Test
## F-Test (Varianz-Vergleich)
Vergleicht die Varianz von 2 Messserien und zeigt somit auf ob systematische Fehler passiert sind.
$$
\begin{gather}
F_{beobachtet} = \frac{s_{A}^2}{s_{B}^2} &mit &  s_{A}^2>s_{B}^2 \implies F_{beobachtet}>1
\end{gather}
$$

Auch hierzu gibt es eine [Referenztabelle](https://statistics.tools/de/f-tabelle) wo $f_{A}=n_{A}-1;f_{B}=n_{B}-1$ gilt.
### Beispiel
|| Labor  1 | Labor 2 |
|------| -------- | ------- |
|Gehalt|0,232%|0,217%|
|$n$|5|3|
|$\sigma$|0,017%|0,0293%|
> Q: Unterscheiden sich die Varianzen signifikant im 95% Vertrauensbereich?
$$
\begin{gather}
\sigma_{1}<\sigma_{2} \\
\implies f = \frac{{\sigma_{2}}^2}{{\sigma_{1}}^2} = 2,97 \\
f_{Tabelle} = 6,994 > f
\end{gather}
$$
> A: Kein signifikanter Unterschied vorhanden.

## T-Test/Student-Test (Mittelwert-Vergleich)
Vergleichstest für Mittelwerte mit einem Sollwert.
$$
\begin{gather}
t = \frac{|\bar{x}-\mu|}{\sigma}*\sqrt{ n } \\
\mu \dots \text{Sollwert}
\end{gather}
$$
Es wird wieder anhand einer Tabelle mit ==$t_{Tabell e}(f=n-1,P\%)$== verglichen, wo $t>t_{Tabelle}$ auf einen Signifikanten Unterschied und $t\leq t_{Tabelle}$ auf einen zufälligen Unterschied hinweist.
> Wie sonst auch $PW>Tabelle$ ist schlecht.

Die [Referenztabelle](https://statistics.tools/de/t-tabelle) nimmt diesmal nur eine Größe als Parameter. $t(f)$
### Beispiel
Sei $n_{1} =3 ;\bar{x}= 0,513\frac{\mu g}{L}$ und $\sigma = 0,05 \frac{\mu g}{L}$ Unterscheidet sich das 5% signifikant von $\mu = 0,52 \frac{\mu g}{L}$ ?
$$
\begin{gather}
t = \frac{|0,513-0,52|}{0,05}*\sqrt{ 3 } = 0,242 \\
t(2;95\%) = 4,303 \\
4,303 > 0,242
\end{gather}
$$
Zufälliger Unterschied.
## Erweiterter T-Test
$$
\begin{gather}
t = \frac{|\bar{x}_{1}-\bar{x}_{2}|}{s_{d}} * \sqrt{ \frac{n_{1}n_{2}}{n_{1}+n_{2}} } \\
s_{d} = \sqrt{ \frac{(n_{1}-1){s_{1}}^2+(n_{2}-1){s_{2}}^2}{n_{1}+n_{2}-2} }
\end{gather}
$$
### Beispiel

> [!Warning]  Vorraussetzung
> Um das machen zu können müssen $s_{1}$ und $s_{2}$ per [[Statistische Tests#F-Test (Varianz-Vergleich)]] vergleichbar sein!

|| Labor  1 | Labor 2 |
|------| -------- | ------- |
|Gehalt|0,232%|0,217%|
|$n$|5|3|
|$\sigma$|0,017%|0,0293%|
1. Wir wissen dass der F-Test keinen signifikanten Unterschied zeigt (siehe bsp F-Test).
2. Erweiterter T-Test

$$
\begin{gather}
s_{d} = \sqrt{ \frac{(5-1){0,017^2+(3-1){0,0293^2}}}{5+3-2} } = 0,022 \\
t = \frac{|0,232-0,217|}{0,022} * \sqrt{ \frac{5*3}{5+3} } = 0,094 \\
t_{tabelle}(n_{1}+n_{2}-2) = 2,447 > 0,094
\end{gather}
$$
Keine signifikanten Unterschiede im Mittelwert.