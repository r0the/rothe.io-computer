# Tetra
---

* [:pdf: Tetra: Informationen (PDF)](./tetra-informationen.pdf)
* [:pdf: Tetra: Komponenten (PDF)](./tetra-komponenten.pdf)
* [:pdf: Tetra: Mikrocode (PDF)](./tetra-mikrocode.pdf)

Das Rollenspiel ist so gestaltet, dass folgende wichtige Erkenntnisse hervorgehoben werden:

**Ebenen:** Das Modell ist auf Ebene der Befehlssatz- und Mikroarchitektur so realistisch und gleichzeitig einfach wie möglich gehalten. Die Ebene der digitalen Logik wird bewusst ausgeblendet.

**Kommunikation:** Die Komponenten kommunizieren ausschliesslich über das Bussystem. Daten- und Adressbus werden im Rollenspiel als zentrales «Register» dargestellt, auf das sämtliche Spieler/innen Zugriff haben. Der Steuerbus wird durch die mündliche Kommunikation der Spieler/innen modelliert.

**Datendarstellung:** Die Darstellung der Daten in Form von Bits soll zeigen, dass der Computer auf der Ebene der Mikroarchitektur eben nicht mit Zahlen rechnet, sondern nur mit zwei Zuständen arbeitet. Wenn die Schüler/innen ein Programm ausführen, so erleben sie, dass sie wir der Computer keine Vorstellung davon haben, was semantisch passiert.

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
LD 6
ADD 7
OUT
```

Das Programm B: Zählen (Länge 10)

```
LD 0
x: ADD 2
OUT
CMP 10
JNE x
HLT
```

Zwei Benutzereingaben addieren (Länge 7)

```
IN
STO B
IN
ADD B
OUT
```

Multiplikation:

```
LD 0
ADD B
STO C
```
