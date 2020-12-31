# Tetra - Beispiele
---

## Addition

Das folgende Programm liest zwei Zahlen ein, addiert sie und gibt das Resultat aus:

```
IN 15
IN 14
LD 15
ADD 14
STO 15
OUT 15
HCF
```

| Speicher | Wert | Bedeutung  |
|:-------- |:---- |:---------- |
| 0        | 0    | IN         |
| 1        | 15   | a          |
| 2        | 0    | IN         |
| 3        | 14   | b          |
| 4        | 2    | LD         |
| 5        | 15   | a          |
| 6        | 3    | ADD        |
| 7        | 14   | b          |
| 8        | 5    | STO        |
| 9        | 15   | a          |
| 10       | 1    | OUT        |
| 11       | 15   | a          |
| 12       |      |            |
| 13       |      |            |
| 14       |      | Variable b |
| 15       |      | Variable a |

## Zwei Zahlen multiplizieren

```
IN 15
IN 14
LD 14
JZ ende
LD 15
ADD 15
STO 15
```
