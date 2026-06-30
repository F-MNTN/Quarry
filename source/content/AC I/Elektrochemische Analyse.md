---
created: 2026-06-27
tags:
  - Chemistry
subject:
  - Analytical Chemistry
  - Basics
---
# Core ideas
Elektroanalytische Methoden verwenden Elektrochemische Vorgänge an oder zwischen Elektroden einer elektrochemischen Zelle zur Gewinnung von Information über eine Probe.
- Sehr hohe Empfindlichkeit
- Bestimmung von Oxidationszuständen möglich 
- Bestimmung von thermodynamischer Aktivität möglich
# Content
## Analysemethoden
### Potentiometrie
#### Elektrochemische Zelle
##### Aufbau
- Anode (hier findet Oxidation statt)
- Kathode (hier findet Reduktion statt)
- Elektrolyt
- Salzbrücke
##### Notation
Reaktanten werden durch $|$ getrennt die zwei Halbzellen werden durch $||$ getrennt.
$$
\begin{gather}
  & \underline{Zn|Zn^{2+}||Cu^{2+}|Cu} \\ 
I: &  {Zn\rightleftharpoons Zn^{2+} + 2e^{-}}  & \text{Anode} \\
II: &  {Cu^{2+} + 2e^- \rightleftharpoons Cu} & \text{Kathode}
\end{gather}
$$
![[Pasted image 20260627192655.png]]
Die Salzbrücke dient nur zum Schluss des Strokreises und lässt nur $e^-$ fließen. 
##### Rechnung
![[Pasted image 20260627193219.png]]
### Konduktometrie
> [!Quote] AC-I Elektrochemische Methoden
>Messung der elektrischen Leitfähigkeit von Elektrolytlösungen. Die  erfasste Ionen-Leitfähigkeit ist – bei nicht zu hohen Konzentrationen – nahezu proportional der Konzentration gelöster Elektrolyte. 

#### Schwache Säure/Starke Base Titration
Die gelösten Protonen $H^+$ steigern die Leitfähigkeit der Lösung. Sobald eine Base mit dem Elektrolyt reagiert sinkt die $H^+$ Konzentration und die Leitfähigkeit sinkt. 
![[Pasted image 20260628151147.png]]
Wie in ``2) im Bild`` geschrieben steigt die Leitfähigkeit wieder langsam sobald sich genug NaAc bildet und dissoziiert. Effektiv entsteht hier ein ${HAc/NaAc}$ [[Puffer#Säurepuffer]]. Auch wenn hier ein Puffer entsteht, er ist nicht direkt der Grund für dieses Verhalten. Grundlage ist die Entstehung von $NaAc$, einen starken Elektrolyt. So lange $NaOH$ noch um gesetzt wird zu $NaAc$ wirkt die Reduktion von freien $H^+$ senkend für die el.-Leitfähigkeit aber wird wegen der Dissoziationsreaktion ${NaAc \rightleftharpoons Na^+ + Ac^-}$, was mehr Ionen in lösung bringt, stärker nach oben getrieben. Dies passiert bis exakt zum *Äquivalenz-Punkt*.
Nach diesem Punkt wird das $NaOH$ nicht mehr neutralisiert, weil keine freien $HAc$ mehr in Lösung sind. Dadurch steigt die Leitfähigkeit wieder stärker. 

#### Fällungstitration
Ähnliches Prinzip gilt bei der Fällungsreaktion:
![[Pasted image 20260628154013.png]]
$$
\begin{gather}
{NaCl + AgNO_{3} \rightleftharpoons AgCl\downarrow + Na^+ + NO^{3-} }
\end{gather}
$$
Schwer lösliches $AgCl$ fällt aus der Lösung bis $n(Cl^-) = n(NO_{3}+)$. Sobald dieser *Äquivalenzpunkt* erreicht ist, ist jedes $Cl^-$ in Form von $AgCl$ ausgefallen und hinzufügen von ${AgNO_{3} \rightleftharpoons Ag^+ + NO^{3-}}$ führt zu erhöhter Ionenpräsenz in der Lösung und somit auch zu erhöhter el.-Leitfähigkeit.
### Elektrogravimetrie
Abscheidung eines Metalls aus wässeriger Lösung durch Elektrolyse. 
> [!Description] Elektrolyse
> Zerlegung eines Stoffes durch anlegen eines elektrischen Stroms
>- Anode: Elektronenakzeptor – Oxidation  
>- Kathode: Elektronendonator – Reduktion
#### Anwendung
- Metalle mit positivem Normal-Potential (E°)
- Trennung von Metallen 
	- durch ausreichend großer Differenz in Potential 
	- durch Zugabe von Komplexbildnern
	- durch simultane Abscheidung an Kathode/Anode

##### Vorteile:
- hohe Empfindlichkeit
- sehr gute Präzision
##### Nachteile:
- hoher Zeitaufwand pro Duchsatz (schlecht skalierbar)
- störung durch $Cl^-$ und $NO_{3}^-$ Ionen.
#### Berechnung
Zusammenhang zwischen abgeschiedener Substanzmenge und der  verbrauchten elektrischen Ladung wird durch das Faraday Gesetz  beschrieben: 
$$
\begin{gather}
m = \frac{M}{z*F}*Q \\
\end{gather}
$$
|Formelzeichen|Bedeutung|Einheit|
|---|---|---|
|$m$|Masse der Umgesetzten Substanz|$g$|
|$M$|molare Masse|$\frac{g}{mol}$|
|$z$|$e^-$-Anzahl pro Teilchenumsatz|$/$|
|$F$|Faraday-Konstante|$96487 \frac{C}{mol}$|
|$Q$|el. Ladung|$C$ oder $A*s$|
#### Aufbau
![[Pasted image 20260628161651.png]]
### Coulometrie
In VO-Unterlagen nicht erklärt.
### Polarographie
In VO-Unterlagen nicht erklärt.