# 3.8 Addierer
---

## Binäre Addition

<VueVideo id="x7ka0QwKciA"/>


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

<VueCircuit id="rothe-half-adder"/>

::: exercise Aufgabe Halbaddierer
Baue den Halbaddierer in CircuitVerse nach und probiere aus, ob die Addition von zwei Bits (inklusive Übertrag) korrekt funktioniert.
:::

## Volladdierer

Ein Halbaddierer addiert also eine einzige Stelle und sorgt dafür, dass der Übertrag für die nächste Stelle mittels zweitem Ausgang bereitsteht.

::: exercise Zusatzaufgabe Volladdierer
Verwende mehrere Halbaddierer und setze sie zu einem 4-Bit-Addierer zusammen. Es sollen also zwei 4-Bit-Zahlen korrekt addiert werden können.
:::
