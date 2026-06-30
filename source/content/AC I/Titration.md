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

[[Säure-Base]]
[[RedOx]]
[[pH-Wert]]
[[Gleichgewichte]]
[[Löslichkeit]]
[[Komplexe]]

# Content

Bestimmung der Konzentration einer Substanz (Analyt) in Lösung mittels hinzufügen einer Substanz (Titrant) mit bekannter Konzentration. Ggf. auch ein [[Titration#Indikator]].
Der Titrationsgrad $\tau$ beschreibt den Fortschritt der Titration.

$$
\begin{gather}
\tau = \frac{n_{Titrant}}{n_{Analyt}}
\end{gather}
$$

## Säure-Base-Titration

Anhand pH - Idikator wird Titrant zu Probe hinzugefügt bis ein gewisser umschlag passiert. Damit weiß man, bie welcher Menge an Titrant die Lösung einen bestimmten pH-Wert erreicht hat. Somit kann man trivialerweise auf die Konzentration des Reagenten in der Probe schließen. Besonders sind hier jedoch Puffer systeme zu beachten, die bei dem Halbtitrationspunkt (50% schwache Säure/Base, 50% Salz) lange den pH-Wert halten und dann relativ schnell wieder ansteigen.
Je nach Titrationsgrad muss einem bewusst sein was gerade vorliegt damit der pH-Wert akkurat berrechnet werden kann. [[pH-Wert]]

## RedOx-Titration

Wird wenn möglich selbst-indizierend angesetzt (zB.: Manganometrie mit $KMnO_{4}$). Ansonsten gibt es ebenfalls [[Titration#Indikator]] die gewisse Potentiale sichtbar machen. DA hier $e⁻$ von Reduktionsmittel zu Oxidationsmittel wandern existiert auch eine Spannung ($V$), die mittels [[RedOx#Nernst-Gleichung]] berechnet werden kann. Besonders sind hier die Verhältnisse der Reagenzien zu beachten um $\tau$ richtig zu berechnen.

## Fällungstitration

Hier wird eine Lösung gesättigt. Essentiell ident zu der [[Löslichkeit#Fällungsreaktion]] nur mit analytischem Hintergrund.

## Komplex-Titration

Bildung eines (stabileren) Komplexes. Wird oft unter verwendung von [[Komplexe#Chelate]] wie EDTA gemacht. Wobei der pH wert zu beachten ist. [[Komplexe#EDTA#pH Einfluss]]

### Titrationsverlauf
![[Pasted image 20260627181731.png]]
## Indikator

Stoffe welche durch eine Farbänderung den Endpunkt einer Titration anzeigen, müssen System-adaptiert sein, d.h. selbst als Säure/Base, Chelatbildner oder Redox-Paar fungieren
zB.:

- S/B
  - Phenolphtahlein
  - Methylorange
- RedOx
  - Manganometrie ($KMnO_{4}$ als Titrant) Ist per se gefärbt aber verliert Farbe wenn reduziert
  - Cerimetrie $Ce^{4+} + e⁻ \rightleftharpoons Ce^{3+}$
  - Dichromatometrie $Cr_{2}O_{7}^{2-} + 14H_{3}O⁺ + 6e⁻ \rightleftharpoons 2Cr^{3+} + 21 H_{2}O$
  - Iodometrie $I_2 + 2e⁻ \rightleftharpoons 2 I⁻$
  - Bromatometrie $BrO_3⁻ + 6 H_3O⁺ + 6e⁻\rightleftharpoons Br⁻ + 9 H_2O$
## Namenstitration
### Chlorid-Titration nach Volhard
Das ist eine  [Indirekte Titration](https://de.wikipedia.org/wiki/Titration#Indirekte_Titration).
Es wird mit einem Überschuss an $AgNO_{3}^-$ reagiert damit $AgCl$ quantitativ ausfällt.
$$
\begin{gather}
I:\ce{Ag+ + Cl- \rightleftharpoons AgCl\downarrow}
\end{gather}
$$
Überschuss an $Ag^+$ wird mit $SCN^-$ rücktitriert.
$$
\begin{gather}
II:\ce{Ag+ + SCN- \rightleftharpoons AgSCN\downarrow}
\end{gather}
$$
Überschuss an $SCN^-$ reagiert zu rotem Eisenkomplex.
$$
\begin{gather}
III: \ce{Fe^3+ + 2SCN- \rightleftharpoons [Fe(SCN)2]+ }
\end{gather}
$$
### Chlorid-Titration nach Mohr
Fällungstitration von $NaCl$ anhand $AgCl$ mit $AgNO_{3}$.
$$
\begin{gather}
I:\ce{NaCl + AgNO3 \rightleftharpoons NaNO3 + AgCl\downarrow}
\end{gather}
$$
Am *Aquivalenzpunkt* gilt $n(Ag^+) = n(Cl^-)$
Überschuss von $Ag^+$ Ionen wird mittels $\ce{CrO4^2-}$ durch Rot-braunen $Ag_{2}CrO_{4}$ Niederschlag indiziert.
$$
\begin{gather}
\ce{2Ag+ + CrO4^2- \rightleftharpoons Ag2CrO4\downarrow}
\end{gather}
$$