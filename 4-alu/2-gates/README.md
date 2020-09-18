# Gatter
---

Die Grundlage der Digitalelektronik bilden Schaltungen, welche einen oder zwei **Eingänge** und einen **Ausgang** haben. Solche Schaltungen heissen **Gatter**.

## AND-Gatter (*AND-gate*)

Ein AND-Gatter ist eine Schaltung, welche zwei Eingänge und einen Ausgang hat. Der Ausgang Y hat nur dann den Wert 1 (hohe Spannung), wenn Eingange A **und** Eingang B den Wert 1 (hohe Spannung) haben.

| A   | B   |   Y |
|:--- |:--- | ---:|
| 0   | 0   |   0 |
| 0   | 1   |   0 |
| 1   | 0   |   0 |
| 1   | 1   |   1 |

In Schaltplänen wird ein AND-Gatter mit folgendem Symbol dargestellt:

![Symbol für ein AND-Gatter](./and-gate.svg)

## OR-Gatter (*OR-gate*)

Bei einem OR-Gatter hat der Ausgang Y dann den Wert 1 (hohe Spannung), wenn Eingang A **oder** Eingang B den Wert 1 (hohe Spannung) haben.

| A   | B   |   Y |
|:--- |:--- | ---:|
| 0   | 0   |   0 |
| 0   | 1   |   1 |
| 1   | 0   |   1 |
| 1   | 1   |   1 |

In Schaltplänen wird ein OR-Gatter mit folgendem Symbol dargestellt:

![Symbol für ein OR-Gatter](./or-gate.svg)

## XOR-Gatter (*XOR-gate*)

Ein XOR-Gatter (engl. *exclusive or*) hat der Ausgang Y dann den Wert 1 (hohe Spannung), wenn Eingang A **oder** Eingang B **aber** nicht beide den Wert 1 (hohe Spannung) haben.

| A   | B   |   Y |
|:--- |:--- | ---:|
| 0   | 0   |   0 |
| 0   | 1   |   1 |
| 1   | 0   |   1 |
| 1   | 1   |   0 |

In Schaltplänen wird ein XOR-Gatter mit folgendem Symbol dargestellt:

![Symbol für ein XOR-Gatter](./xor-gate.svg)

## Inverter

Ein Inverter ist eine Schaltung, bei welcher der Ausgang Y den Wert 1 (hohe Spannung) hat, wenn der Eingang den Wert 0 (tiefe Spannung) hat und umgekehrt.

| A   |   Y |
|:--- | ---:|
| 0   |   1 |
| 1   |   0 |

In Schaltplänen wird ein Inverter mit folgendem Symbol dargestellt:

![Symbol für einen Inverter](./inverter.svg)

## NAND-Gatter (*NAND-gate*)

Ein NAND-Gatter (engl. *not and*) hat der Ausgang Y dann den Wert 0 (tiefe Spannung), wenn Eingange A **und** Eingang B den Wert 1 (hohe Spannung) haben.

| A   | B   |   Y |
|:--- |:--- | ---:|
| 0   | 0   |   1 |
| 0   | 1   |   1 |
| 1   | 0   |   1 |
| 1   | 1   |   0 |

In Schaltplänen wird ein NAND-Gatter mit folgendem Symbol dargestellt:

![Symbol für ein NAND-Gatter](./nand-gate.svg)

Das NAND-Gatter hat eine besondere Bedeutung. Dank dem Mathematiker George Boole kann bewiesen werden, dass **jede** logische Schaltung ausschliesslich aus NAND-Gatter aufgebaut werden kann. Ausserdem sind NAND-Gatter physikalisch relativ einfach aufzubauen. Deshalb bilden NAND-Gatter den Grundbaustein für heutige Mikrochips.
