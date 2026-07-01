---
created: 2026-01-20
tags:
  - Chemistry
subject:
  - Analytical Chemistry
  - Basics
---
# Core ideas

[[AC I Overview]]

# Content

Sind prozesse bei denen e⁻ entzogen/hinzugefügt werden. Dies muss nicht formal komplett passieren. Es kann sich auch um eine partielle verschiebung bei neuer Bindung handeln, sodass ein Atom eine neue Partialladung bekommt.
Bsp: $S + O_{2} \to SO_{2}$ geht von $S,O_{2}$ je mit [[Oxidationszahlen bestimmen]] = 0 zu $SO_{2}$ mit Oxidationszahlen +IV für $S$ und -II für $O_{2}$
Hier wird $S$ oxidiert (Oxidationszahl geht rauf, $S$ ist Reduktionsmittel) und $O$ reduziert (Oxidationszahl geht runter, $O$ ist Oxidationsmittel).
Insgesamt ist die Oxidationszahl eines Moleküls immer gleich seiner Ladung.
Oxidation/Reduktion können _NIE_ alleine auftreten! Sie brauchen einander um reagieren zu können.

## Reduktion

Prozess bei dem e⁻ einem Atom hinzugefügt werden
Die Oxidationszahl sinkt. Das reduzierte Molekül heißt Oxidationsmittel

## Oxidation

Prozess bei dem e⁻ einem Atom entzogen werden.
Die Oxidationszahl steigt. Das oxidierte Molekül heißt Reduktionsmittel.

## RedOx Reaktion aufstellen

1. Edukte und Produkte die beteiligt sind aufstellen. $A + B \to C + D$ und [[Oxidationszahlen bestimmen]].
2. Stöchimetrie anhand der Oxidationszahlen (under deren Änderungen) balancieren.
3. Je nach Milieu mit H⁺(sauer) oder OH⁻(basisch) Ladungen ausgleichen und entsprechend $H_{2}O$ auf die andere seite geben.

### Bsp in sauerer Lösung

$$
\begin{gather}
1: & I_{2} + ClO_{3}⁻ \to IO_{3}⁻ + Cl⁻ \\
Ox: & I:0 \\
 & Cl:+V \to\\
 & I:+V \\
 & Cl:-I \\
2: & 3I_{2} + 5ClO_{3}⁻ \to 6IO_{3}⁻ + 5Cl⁻ \\
3: & 3I_{2} + 5ClO_{3}⁻ + 3H_{2}O \to 6IO_{3}⁻ + 5Cl⁻ + 6H⁺\\
\end{gather}
$$

### Bsp in basischer Lösung

$$
\begin{gather}
1: & MnO_{4}^- + N_{2}H_{4} \to MnO_{2} + N_{2} \\
Ox: & Mn:+VII \\
 & N:-II \to\\
 & MnO:+IV \\
 & N:0 \\
2: & 2MnO_{4}^- + N_{2}H_{4} \to 2MnO_{2} + N_{2} \\
3: & 2MnO_{4}^- + \frac{3}{2}N_{2}H_{4} \to 2MnO_{2} + \frac{3}{2}N_{2} + 2OH^{-} + 2H_{2}O\\
= & 4MnO_{4}^- + 3N_{2}H_{4} \to 4MnO_{2} + 3N_{2} + 4OH^{-} + 4H_{2}O\\
\end{gather}
$$

## Nernst Gleichung

Da bei RedOx Reaktionen $e⁻$ wandern (Strom fließt), gibt es auch Potential unterschiede und somit Spannung. Diese Spannung wird in $e⁻V$ - Elektronenvolt angegeben. In der Regel beschreibt die Nernst Gleichung dieses Verhalten:

$$
\begin{gather}
E = E_0 + \frac{R*T}{z*F}* log\left(\frac{[Ox]}{[Red]}\right) \approx E_0 + \frac{0,059}{z}* log\left(\frac{[Ox]}{[Red]}\right) & \text{bei } 25°C
\end{gather}
$$

Wobei zu beachten ist, dass man hier nur von der umgesetzten Substanz redet. ZB. bei $MnO_{4}⁻ + 5 Fe^{2+} + 8H⁺ \to Mn^{2+} + 5 Fe^{3+} + 4H_{2}O$ ist _$z = 1$_, weil: $Fe^{2+} \to Fe^{3+} + e⁻$.
Im weiteren bezieht sich $log\left(\frac{[Ox]}{[Red]}\right)$ auf den Anteil von $Fe$ der Oxidiert ($Fe^{2+}$)/Reduziert ($Fe^{3+}$) ist. Was sich je nach molarität der Reagenten ändert.

Die Approximation is gut genug.

| Zeichen | Name                    | Bedeutung                              |
| ------- | ----------------------- | -------------------------------------- |
| E       | Reaktionspotential      | Ladung bei $\tau = 1$                  |
| E_0     | Standardpotential       | Ladung bei $\tau = 0$                  |
| z       | $e⁻$ Anzahl             | Anzahl an wandernden $e⁻$              |
| [Ox]    | oxidiertes Mittel       | Konzentration der oxidierten Substanz  |
| [Red]   | reduziertes Mittel      | Konzentration der reduzierten Substanz |
| R       | Avogadro-Zahl           | $8,314 \frac{J}{mol*K}$                |
| T       | Temperatur (meist 25°C) | in $°K$                                |
| F       | Faraday Konstante       | Ladung von 1 mol $e⁻$                  |
