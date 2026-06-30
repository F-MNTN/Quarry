---
created: 2026-02-20
tags:
  - Chemistry
  - Wiki
subject:
  - Analytical Chemistry
  - Basics
---
# Core ideas

[[AC I Overview]]

# Content

Die Eigenschaft eines Feststoffes als Ion sich in flüssiger Phase zu verteilen.

## Ionenprodukt
Im Allgemeinen ist das Ionenprodukt das Produkt der Konzentrationen der gelösten Ionen. 
Für eine Reaktion $\ce{aA + bB \leftrightharpoons cC + dD}$ wird das Ionenprodukt berechnet über das Massenwirkungsgesetz als:
$$
\begin{gather}
K = \frac{[D]^d *[C]^c}{[A]^a*[B]^b} \\ \\
I = K * [A]^a*[B]^b = [D]^d *[C]^c
\end{gather}
$$
## Löslichkeitsprodukt

$$
\begin{gather}
[A + B]_{f} \leftrightharpoons aA + bB\\
K_{L}=c_{A}^{a} * c_{B}^{b} \\
L = \sqrt[a+b]{\frac{K_{L}}{a^{a}*b^{b}}}
\end{gather}
$$

### Unterschied Ionenprodukt $I$ und Löslichkeitsprodukt $L$/$K_{L}$
Die Formel der allgemeinen berechnung ist gleich (wie oben zu sehen ist)
> [!Example] Reaction
> $\ce{aA_{(s)} \leftrightharpoons bB_{(aq)} + cC_{(aq)}}$ wobei $B$ und $C$ die Ionen sind in die $A$ sich löst. 
> >Für $A$ = NaCl => $\ce{B=Na+ C=Cl-}$
> 
> $L = K_{L} = [C]^c*[B]^b$
> $I=[C]^c*[B]^b$

Aber das Löslichkeitsprodukt $L$ nimmt an, dass die Reaktion in GGW ist! Also dass die Lösung gesättigt ist. 
Also:
$$
\begin{gather}
I = L
\end{gather}
$$
die Lösung ist perfekt gesättigt. Und zu diesem Zeitpunkt stimmen dann auch die Formeln überein.

DIe Formel des Ionenprodukts ignoriert das komplett und gibt dir genau das was du ausrechnest. Somit kann mit über den $pK_{L}$ wert eines Salzes $L$ ausgerechnet werden (defacto der Punkt wo $I=L$, die Lösung also gesättigt ist) und über $I$ dann bestimmt werden ob das überschritten wird oder nicht. 

## Fällungsreaktion

Hier wird das Verhältnis der Ionenprodukt und Löslichkeitsprodukt so beeinflusst, dass es zu einem der folgenden Fälle kommt:

| Verhältnis | Folge                                |
| ---------- | ------------------------------------ |
| $I>L$      | Lösung übersättigt $\to$ Ion fällt aus |
| $I=L$      | Lösung gesättigt                     |
| $I<L$      | Ion komplett gelößt                  |

### Beispiel

$$
\begin{gather}
L_{CaF_{2}} = 3,5 * 10^{-11} \frac{mol^{3}}{L^{3}} \\ \\
\ce{CaF2(s) \leftrightharpoons Ca^2+(aq) + 2F⁻(aq)} \\
c(F⁻) = 2c(Ca^{2+}) \\
L = c(Ca^{2+}) * c(F⁻)^{2} = c(Ca^{2+}) * 2^{2} * c(Ca^{2+})^{2} = 4 * c(Ca^{2+})^{3} = 3,5 * 10^{-11} \\
\implies c(Ca^{2+}) = \frac{\sqrt[3]{3,5 * 10^{-11}}}{4} = 2,1 * 10^{-4}\frac{mol}{L} \\
\implies c(F⁻) = 2c(Ca^{2+}) = 4,2 * 10^{-4}\frac{mol}{L} \\
c(CaF_{2}) = 2,1 * 10^{-4}\frac{mol}{L}\\
\end{gather}
$$

Es sind $c(CaF_{2}) = 2,1 * 10^{-4}\frac{mol}{L}$ in Lösung.

Wie viel  g $CaF_{2}$ in 100ml?

$$
\begin{gather}
n(CaF_{2}) = c(CaF_{2}) * V = 2,1 * 10^{-4}\frac{mol}{L} * 0,1L = 2,1*10^{-5}mol\\
m(CaF_{2}) = n(CaF_{2}) * M(CaF_{2}) = 2,1*10^{-5} * 78 \frac{g}{mol} = 1,6 * 10^{-3}g
\end{gather}
$$

## pH-Abhängige Fällung
https://www.youtube.com/watch?v=G5FVxAzlmfM