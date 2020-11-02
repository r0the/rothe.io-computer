# 3.8 Addierer
---

## Binäre Addition

<VueVideo id="x7ka0QwKciA"/>

::: exercise
Führe eine schriftliche Addition für die folgenden binären Zahlen durch:

- $1001_2 + 110_2$
- $111_2 + 1_2$
- $101_2 + 101_2$

:::

## Halbaddierer

Wie könnte man die Addition zweier einstelliger Zahlen im Binärsystem als Schaltung konstruieren?

$$\begin{aligned}
0 + 0 &= 00_2\\
0 + 1 &= 01_2\\
1 + 0 &= 01_2\\
1 + 1 &= 10_2
\end{aligned}$$

Die entsprechende Schaltung benötigt zwei Eingänge und zwei Ausgänge. Die beiden Eingänge werden für die zwei Summanden verwendet. Die Ausgänge für die Einer- und Zweierstelle des Resultats. Die gesuchte Schaltung muss also folgende Wertetabelle haben:

| A   | B   | Zweier | Einer |
|:--- |:--- | ------:| -----:|
| 0   | 0   |      0 |     0 |
| 0   | 1   |      0 |     1 |
| 1   | 0   |      0 |     1 |
| 1   | 1   |      1 |     0 |

Der Wert der Einerstelle kann durch ein XOR-Gatter berechnet werden, der Wert der Zweierstelle durch ein AND-Gatter. Die Schaltung sieht somit so aus:

<VueCircuit id="rothe-half-adder-vertical"/>

## Volladdierer

Wenn zwei mehrstellige binäre Zahlen addiert werden sollen, muss zusätzlich der **Übertrag** berücksichtigt werden. Ab der zweithintersten Stelle muss folgendermassen vorgegangen werden:

1. Die Zifferen an der aktuellen Stelle werden addiert.
2. Zum Resultat wird der Übertrag der vorherigen Stelle addiert.
3. Die höhere Stelle des Resultat wird als Übertrag an die nächste Stelle weitergegeben.

Dies kann mit der folgenden Schaltung realisiert werden. Sie besteht aus zwei Halbaddierern sowie einem OR-Gatter. Mit dem OR-Gatter werden die beiden möglichen Überträge zusammengefasst.

<VueCircuit id="rothe-full-adder-vertical"/>

Um zwei binäre Zahlen von beliebiger Länge zu addieren, können Volladdierer beliebig aneinandergehängt werden:

<VueCircuit id="rothe-four-bit-adder"/>

::: exercise Aufgabe
Erstelle eine Wahrheitstabelle für den Volladdierer. Der Volladdierer hat drei Eingänge:
- A (erste Zahl)
- B (zweite Zahl)
- U (Übertrag)

und zwei Ausgänge:

- Y (Resultat)
- V (Übertrag)
:::
