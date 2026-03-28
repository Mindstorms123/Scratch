# 🏁 Scratch 2-Spieler-Rennspiel

![Projekt-Vorschau](https://github.com/user-attachments/assets/facfab1d-afa7-484f-ad1a-5e85955aa2ab)

Dieses Projekt ist ein einfaches, actionreiches 2-Spieler-Rennspiel, das in Scratch entwickelt wurde. Es wurde speziell für eine Schulung im Rahmen des **Diesterweg-Stipendiums (5. Klasse)** konzipiert.

Zwei Spieler rasen auf einer runden Strecke gegeneinander – wer zuerst die Zielflagge berührt, gewinnt!

## ✨ Features

* 👥 **Lokaler Mehrspieler:** Trete direkt gegen einen Freund an demselben Computer an.
* 🏎️ **Gleichzeitiges Lenken & Fahren:** Volle Kontrolle! Vorwärts/rückwärts fahren und gleichzeitig drehen ist möglich.
* ⏱️ **Integrierter Timer:** Eine laufende Stoppuhr oben links zeigt die Rennzeit.
* 🏆 **Gewinn-Bedingung:** Bei Berührung der Zielflagge wird sofort das Siegesbild für den entsprechenden Spieler angezeigt.
* 🎨 **Custom Pixel-Art Assets:** Maßgeschneiderte Rennwagen (Rot & Gelb) und eine passende Rennstrecke.

## 🕹️ Steuerung

Beide Spieler können gleichzeitig steuern:

| Spieler / Aktion | ⬆️ Vorwärts | ⬇️ Rückwärts | ⬅️ Links drehen | ➡️ Rechts drehen |
| :--- | :---: | :---: | :---: | :---: |
| **Rot** (Pfeiltasten) | `Pfeil Oben` | `Pfeil Unten` | `Pfeil Links` | `Pfeil Rechts` |
| **Gelb** (WASD) | `W` | `S` | `A` | `D` |

---

## 🛠️ Installation & Start

Befolge diese einfachen Schritte, um das Spiel in Scratch zu bauen:

1.  **Scratch öffnen:** Gehe zu [scratch.mit.edu](https://scratch.mit.edu) und klicke auf "Entwickeln", um ein neues Projekt zu erstellen.
2.  **Assets hochladen:** Lade die generierten Bilder (aus dem `assets`-Ordner) hoch:
    * **Rennstrecke:** Als Hintergrund hochladen.
    * **Rotes Auto:** Als neues Sprite hochladen.
    * **Gelbes Auto:** Als neues Sprite hochladen.
    * **Gewinn-Bilder (Rot/Gelb):** Als neue Hintergründe oder Sprites hochladen.
3.  **Scripte kopieren:** Baue die untenstehenden Code-Blöcke für die jeweiligen Sprites nach (oder kopiere sie aus den Screenshots).
4.  **Rennen starten:** Klicke auf die **grüne Flagge** 🟢 – los geht's!

---

## 💻 Die wichtigsten Scripts

Hier sind die Kern-Logikblöcke für das Spiel.

### 🚗 Für beide Autos (Beispiel Rot)

*Passe die Tasten und Startposition für das gelbe Auto entsprechend an.*

```scratch
wenn [grüne Flagge] angeklickt
gehe zu x: (-180) y: (50) // Startposition Rot
setze Richtung auf (90) Grad
wiederhole fortlaufend
  falls <Taste [Pfeil nach oben v] gedrückt?>, dann
    gehe (3) er Schritt
  ende
  falls <Taste [Pfeil nach unten v] gedrückt?>, dann
    gehe (-2) er Schritt
  ende
  falls <Taste [Pfeil nach links v] gedrückt?>, dann
    drehe dich ↺ um (5) Grad
  ende
  falls <Taste [Pfeil nach rechts v] gedrückt?>, dann
    drehe dich ↻ um (5) Grad
  ende
  falls <wird [Zielflagge v] berührt?>, dann
    sende [Rot gewinnt v] an alle
    stoppe [alles v]
  ende
ende
