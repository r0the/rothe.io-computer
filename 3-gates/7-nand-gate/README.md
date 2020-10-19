# 3.7 NAND-Gatter
---

Ein NAND-Gatter (engl. *not and*) hat der Ausgang Y dann den Wert 0 (tiefe Spannung), wenn Eingange A **und** Eingang B den Wert 1 (hohe Spannung) haben.

|  A  |  B  |  Y  |
|:---:|:---:|:---:|
|  0  |  0  |  1  |
|  0  |  1  |  1  |
|  1  |  0  |  1  |
|  1  |  1  |  0  |

In Schaltplänen wird ein NAND-Gatter mit folgendem Symbol dargestellt:

![Symbol für ein NAND-Gatter](./nand-gate.svg)

## Interaktive Schaltung

<VueCircuit id="rothe-nand-gate"/>

Ein NAND-Gatter kann aus einem AND-Gatter, gefolgt von einem Inverter zusammengesetzt werden:

![](./nand-circuit.svg)

::: exercise Aufgaben
1. TODO
2. Eine Schleuse in einem Hochsicherheitslabor hat 2 Türen. Es dürfen nicht beide Türen gleichzeitig geöffnet werden können. An jeder Türe gibt es einen Druckknopf, der bei geschlossener Tür aktiviert wird. Entwirf die Schaltung mit zwei _Buttons_ und einem _Output_, der angibt, ob momentan eine Tür geöffnet werden darf (Ausgabe **1**) oder nicht (Ausgabe **0**).

    ![](./ex-security-gate.svg)

:::

::: info Universalgatter

Das NAND-Gatter hat eine besondere Bedeutung. Dank dem Mathematiker George Boole kann bewiesen werden, dass **jede** logische Schaltung ausschliesslich aus NAND-Gatter aufgebaut werden kann. Ausserdem sind NAND-Gatter physikalisch relativ einfach aufzubauen. Deshalb bilden NAND-Gatter den Grundbaustein für heutige Mikrochips.
:::
