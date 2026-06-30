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

Auch hierzu gibt es eine Referenztabelle wo $f_{A}=n_{A}-1;f_{B}=n_{B}-1$ gilt.
![[Pasted image 20260626170408.png]]
### Beispiel
![[Pasted image 20260626170637.png]]

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
### Beispiel
![[Pasted image 20260626173105.png]]
![[Pasted image 20260626173135.png]]
## Erweiterter T-Test
$$
\begin{gather}
t = \frac{|\bar{x}_{1}-\bar{x}_{2}|}{s_{d}} * \sqrt{ \frac{n_{1}n_{2}}{n_{1}+n_{2}} } \\
s_{d} = \sqrt{ \frac{(n_{1}-1){s_{1}}^2+(n_{2}-1){s_{2}}^2}{n_{1}+n_{2}-2} }
\end{gather}
$$
### Beispiel
==Um das machen zu können müssen $s_{1}$ und $s_{2}$ per [[Statistische Tests#F-Test (Varianz-Vergleich)]] vergleichbar sein!==
![[Pasted image 20260626173840.png]]