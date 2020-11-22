# 4.4 Von-Neumann-Zyklus
---

Der Prozessor führt immer wieder den gleichen zyklischen Ablauf aus. Dieser Ablauf wird auch **Von-Neumann-Zyklus** genannt und besteht aus folgenden vier Schritten:

![](./cycle.svg)

## Befehlsadresse setzen

Die Speicheradresse, an welcher der nächste Befehl steht, wird vom Befehlszähler an das Speicherwerk übermittelt.

![](./step-1.svg)

## Befehl abrufen

Der Befehl wird aus dem Speicher über den Datenbus in das Dekodierwerk übertragen.

![](./step-2.svg)

## Programmzähler erhöhen

Damit im nächsten Durchlauf der nächste Befehl geladen wird, muss der Programmzähler um eins erhöht werden.

![](./step-3.svg)

## Befehl decodieren

Das Dekodierwerk setzt den Befehl in Steuersignale an die verschiedenen Komponenten um.

![](./step-4.svg)

## Datenadresse setzen

Manche Befehle verwenden Daten aus dem Speicher. Bevor der Befehl ausgeführt wird muss daher dem Speicherwerk die Adresse der Speicherzelle mitgeteilt werden.

## Befehl ausführen

Ein Wert wird aus dem Speicher geladen oder in den Speicher geschrieben. Das Rechenwerk führt die arithmetische Operation aus.
