# Tetra
---

* [:pdf: Tetra: Komponenten (PDF)](./tetra-komponenten.pdf)
* [:pdf: Tetra: Mikrocode (PDF)](./tetra-mikrocode.pdf)

Das Rollenspiel ist so gestaltet, dass folgende wichtige Erkenntnisse hervorgehoben werden:

**Ebenen:** Das Modell ist auf Ebene der Befehlssatz- und Mikroarchitektur so realistisch und gleichzeitig einfach wie möglich gehalten. Die Ebene der digitalen Logik wird bewusst ausgeblendet.

**Kommunikation:** Die Komponenten tauschen Daten und Adressen ausschliesslich über den Bus aus. Daten- und Adressbus werden im Rollenspiel als zentrales «Register» dargestellt, auf das sämtliche Spieler/innen Zugriff haben. Der Steuerbus wird durch die mündliche Kommunikation der Spieler/innen modelliert.

## Rollenverteilung

Die Verteilung der Aufgaben auf die verschiedenen Rollen ist so gehalten, dass die Arbeitsteilung nicht zu einseitig ist. Es gibt aber klar eine Hierarchie der Rollen nach absteigenden Anforderungen:

| Rolle        | Anforderungen                      |
| ------------ | ---------------------------------- |
| Dekodierer   | kann Überblick bewahren            |
| Taktgeber    | kann Überblick bewahren            |
| Rechenwerk   | kann 4-Bit-Operationen durchführen |
| Adressierer  | kann Inkrement durchführen         |
| Speicherwerk | -                                  |
| Benutzer     | -                                  |

Die Rolle des Benutzers kann auch weggelassen werden.


## Anwendungsmöglichkeiten

Das Rollenspiel bietet Anwendungsmöglichkeiten auf verschiedenen Ebenen der kognitiven Prozessdimension, beispielsweise:

- **Verstehen:** Vorgegebenes Programm mit Beschreibung ausführen, anschliessend Bedeutung der Einzelschritte besprechen.

- **Analysieren:** Vorgegebenes Programm ohne Erläuterung ausführen, anschliessend herausfinden, was die Intention des Programms ist.

- **Erschaffen:** Zusätzliche Instruktion (z.B. Subtraktion) für den Modellrechner entwerfen und auf die bestehenden Mikroinstruktionen zurückführen.

## Programme

Das Programm A: Zwei Konstanten addieren (Länge 5)

```
LDI 6
ADI 7
OUT
HCF
```

Speicher:

```
6, 6, 8, 7, 2, 0
```

Das Programm B: Zählen (Länge 10)

```
LDI 0
x: ADI 2
OUT
SBI 10
JLS x
HCF
```

Speicher:

```
TODO 6, 0, 8, 2, 2, 10, 10,
```

Zwei Benutzereingaben addieren (Länge 7)

```
INP
STO B
IN
ADD B
OUT
HCF
```

Speicher:

```
1, 12, 15, 1, 9, 15, 2, 0
```

Multiplikation:

```
LD 0
ADD B
STO C
```

TODO:

- Input und Output in Speicher
- "Lese Datenbus" statt "Lese"
- 
