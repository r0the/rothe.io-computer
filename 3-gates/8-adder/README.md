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

## Volladdierer

TODO
