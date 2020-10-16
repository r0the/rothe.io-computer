# Schaltung
---

Im folgenden betrachten wir digitale **Schaltungen**. Eine digitale Schaltung hat einen oder mehrere Eingänge und Ausgänge. Da die Schaltung digital ist, sind bei jedem Eingang und Ausgang immer nur zwei Werte möglich: Null oder Eins.

![](./blackbox.svg)

## Eingabe

Um einfache Schaltungen erstellen zu können, benötigen wir ein paar einfachen Ein- und Ausgabemöglichkeiten.  Wir haben folgende Eingabemöglichkeiten für unsere Schaltungen:

|                               |                                                                        |
| ----------------------------- | ---------------------------------------------------------------------- |
| ![](./sensor-button.svg)      | Druckknopf, liefert Eingabe **Eins**, wenn er gedrückt wird.           |
| ![](./sensor-temperature.svg) | Temperatursensor, liefert als Eingabe **Eins**, wenn es warm ist.      |
| ![](./sensor-light.svg)       | Lichtsensor, liefert als Eingabe **Eins**, wenn es hell ist.           |
| ![](./sensor-humidity.svg)    | Feuchtigkeitssensor, liefert als Eingabe **Eins**, wenn es feucht ist. |

Für die Ausgabe stehen folgende Geräte zu Verfügung:

|                         |                                         |
| ----------------------- | --------------------------------------- |
| ![](./actor-light.svg)  | Licht, brennt bei Ausgabe **Eins**      |
| ![](./actor-sound.svg)  | Lautsprecher, tönt bei Ausgabe **Eins** |
| ![](./actor-heater.svg) | Heizung, heizt bei Ausgabe **Eins**     |
| ![](./actor-motor.svg)  | Motor, läuft bei Ausgabe **Eins**       |


## Direkte Verbindung

Die einfachste Schaltung ist die direkte Verbindung zwischen Ein- und Ausgabe. Betrachten wir ein paar Beispiele:

### Türklingel

Es klingelt, wenn die Taste gedrückt wird.

![](./door-bell.svg)

### Feueralarm

Wenn es brennt (zu hohe Temperatur), so soll ein Warnlicht angeschaltet werden und ein akustisches Signal ertönen.

![](./fire-alarm.svg)
