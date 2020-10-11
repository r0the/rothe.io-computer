# 1.3 Prozessor
---

Der Prozessor ist für die **Verarbeitung** von Daten im Computer zuständig. Ausserdem überwacht und steuert er den Ablauf von Programmen.

Moderne Prozessoren enthalten mehrere **Kerne**, welche unabhängig voneinander Programme ausführen und Berechnungen vornehmen können.

## Kenngrössen

Für den Prozessor gibt es folgende wichtige Kenngrössen:

- Die Anzahl **Kerne** gibt an, wie viele Berechnungen ein Prozessor gleichzeitig ausführen kann.
- Die **Taktfrequenz** gibt an, wie schnell der Prozessor Berechnungen durchführen kann. Sie wird in der Einheit **Hertz** angegeben, was «pro Sekunde» bedeutet.

::: columns 3
![AMD Ryzen-Prozessor ©](./cpu-top.png)
***
![Pins auf Unterseite ©](./cpu-bottom.png)
***
![geöffneter Prozessor ©](./cpu-open.png)
:::

## Aufgaben

Der Prozessor hat zwei Hauptaufgaben. Einerseits **kontrolliert** er die Ausführung der Programmanweisungen. Dabei **steuert** er alle anderen Komponenten des Computers.

Andererseits **verarbeitet** der Prozessor Daten. Das heisst, er führt mathematische oder logische Operationen mit binären Zahlen aus, beispielsweise:

- Vergleichen
- Addieren
- Multiplizieren
- Bits um eine Stelle nach links schieben

Im Kapitel [Rechnerarchitektur](?page=2-0-architecture) wird die Funktionsweise des Prozessors genauer erklärt.

## Weitere Funktionen

Im moderne Prozessor-Chips werden auch weitere Funktionen integriert, welche früher von separaten Bauteilen übernommen wurden.

Moderne Desktop-Prozessoren enthalten normalerweise eine Grafikeinheit, welche die Darstellung von Text, Bild und Video auf einem Bildschirm übernimmt.

Bei Prozessoren für Mobiltelefon werden üblicherweise spezialisierte Funktionen für GPS, W-LAN, Mobilfunk und Bluetooth auf dem Chip integriert. Dabei spricht man von einem Ein-Chip-System oder SoC (engl. *system on a chip*).

## Transistor

Ein **Transistor** ist ein elektronisches Bauelement, mit welchem Spannungen gesteuert werden können. Es sind also elektronische «Schalter». Sämtliche digitalen Schaltungen in Computerchips werden aus Transistoren zusammengesetzt. Die Schaltungen werden mittels einem Fotolitografie-Verfahren erstellt.

Mit dem modernsten 5-Nanometer-Verfahren können bis zu 170 Millionen Transistoren auf einen Quadratmillimeter aufgebracht werden.

## Mooresches Gesetz[^1]

Das mooresche Gesetz besagt, dass sich die Anzahl Transistoren, welche auf einem Computerchip Platz finden, regelmässig verdoppelt. Je nach Quelle werden 12, 18 oder 24 Monate als Zeitraum genannt.

![Entwicklung der Anzahl Transistoren in Desktop-Prozessoren[^2] ©](./moores-law.png)


::: exercise Aufgaben Prozessor
1. Prozessoren sind «Multitasking»-fähig. Wie kann ein Prozessor (resp. ein Kern alleine) mehrere Dinge «gleichzeitig» tun?
:::


[^1]: Quelle: [Wikipedia: Moorsches Gesetz](https://de.wikipedia.org/wiki/Mooresches_Gesetz)
[^2]: Datenquelle: [Wikipedia: Transistor Count](https://en.wikipedia.org/wiki/Transistor_count)
