# Weitere Gatter
---

## NAND-Gatter (*NAND-gate*)

Ein NAND-Gatter (engl. *not and*) hat der Ausgang Y dann den Wert 0 (tiefe Spannung), wenn Eingange A **und** Eingang B den Wert 1 (hohe Spannung) haben.

|  A  |  B  |  Y  |
|:---:|:---:|:---:|
|  0  |  0  |  1  |
|  0  |  1  |  1  |
|  1  |  0  |  1  |
|  1  |  1  |  0  |

In Schaltplänen wird ein NAND-Gatter mit folgendem Symbol dargestellt:

![Symbol für ein NAND-Gatter](./nand-gate.svg)

Ein NAND-Gatter kann aus einem AND-Gatter, gefolgt von einem Inverter zusammengesetzt werden:

![](./nand-circuit.svg)

::: info Universalgatter

Das NAND-Gatter hat eine besondere Bedeutung. Dank dem Mathematiker George Boole kann bewiesen werden, dass **jede** logische Schaltung ausschliesslich aus NAND-Gatter aufgebaut werden kann. Ausserdem sind NAND-Gatter physikalisch relativ einfach aufzubauen. Deshalb bilden NAND-Gatter den Grundbaustein für heutige Mikrochips.
:::

## XOR-Gatter

Ein XOR-Gatter (engl. *exclusive or*) hat der Ausgang Y dann den Wert 1 (hohe Spannung), wenn Eingang A **oder** Eingang B **aber** nicht beide den Wert 1 (hohe Spannung) haben.

|  A  |  B  |  Y  |
|:---:|:---:|:---:|
|  0  |  0  |  0  |
|  0  |  1  |  1  |
|  1  |  0  |  1  |
|  1  |  1  |  0  |

In Schaltplänen wird ein XOR-Gatter mit folgendem Symbol dargestellt:

![Symbol für ein XOR-Gatter](./xor-gate.svg)
