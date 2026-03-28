# 🏁 Scratch 2-Spieler-Rennspiel

![Projekt-Vorschau](https://github.com/user-attachments/assets/facfab1d-afa7-484f-ad1a-5e85955aa2ab)

Dieses Projekt ist ein einfaches, actionreiches **2-Spieler-Rennspiel** in Scratch. Es wurde speziell für eine Schulung im Rahmen des **Diesterweg-Stipendiums (5. Klasse)** entwickelt.

Zwei Spieler rasen auf einer runden Strecke gegeneinander – wer zuerst die Zielflagge berührt, gewinnt! 🏆

---

## ✨ Features

- 👥 **Lokaler Mehrspieler** – Trete direkt gegen einen Freund am gleichen Computer an
- 🏎️ **Gleichzeitiges Lenken & Fahren** – Volle Kontrolle über Richtung und Geschwindigkeit
- ⏱️ **Integrierter Timer** – Stoppuhr oben links zeigt die aktuelle Rennzeit
- 🎯 **Gewinn-Bedingung** – Sofortiges Gewinn-Feedback bei Zielflaggen-Berührung
- 🎨 **Custom Pixel-Art Assets** – Maßgeschneiderte Rennwagen (Rot & Gelb) und Rennstrecke

---

## 🕹️ Steuerung

Beide Spieler steuern **gleichzeitig**:

| Spieler | Vorwärts | Rückwärts | Links drehen | Rechts drehen |
|---------|----------|-----------|--------------|---------------|
| **Rot** | `↑` | `↓` | `←` | `→` |
| **Gelb** | `W` | `S` | `A` | `D` |

---

## 🚀 Installation & Start

### Schritt-für-Schritt-Anleitung

1. **Scratch öffnen**
   - Gehe zu [scratch.mit.edu](https://scratch.mit.edu)
   - Klicke auf „Entwickeln"

2. **Assets hochladen**
   - **Rennstrecke** → Als neuer Hintergrund
   - **Rotes Auto** → Als neues Sprite
   - **Gelbes Auto** → Als neues Sprite
   - **Gewinn-Bilder** → Als Hintergründe oder Sprites

3. **Scripte programmieren**
   - Folge der Logik in Abschnitt [Die wichtigsten Scripts](#-die-wichtigsten-scripts)

4. **Spielen!**
   - Klicke die **grüne Flagge** 🟢 und los geht's!

---

## 💻 Die wichtigsten Scripts

### 🚗 Bewegungs-Logik für rotes Auto

wenn [grüne Flagge] angeklickt
gehe zu x: (-180) y: (50)
setze Richtung auf (90) Grad

wiederhole fortlaufend
falls <Taste [Pfeil nach oben ▲] gedrückt?> dann
gehe (3) er Schritt
ende


falls <Taste [Pfeil nach unten ▼] gedrückt?> dann
  gehe (-2) er Schritt
ende

falls <Taste [Pfeil nach links ◀] gedrückt?> dann
  drehe dich ↺ um (5) Grad
ende

falls <Taste [Pfeil nach rechts ▶] gedrückt?> dann
  drehe dich ↻ um (5) Grad
ende

falls <wird [Ziellinie (gelb)] berührt?> dann
  sende [Rot gewinnt v] an alle
  stoppe [alles v]
ende
ende
ende



**Für gelbes Auto:** Passe die Startposition (z. B. `(180), (50)`) und Tasten (W, A, S, D) an.

---

### ⏱️ Timer-Logik

wenn [grüne Flagge] angeklickt
stoppuhr zurücksetzen

wiederhole fortlaufend
sage (runde [stoppuhr v])
ende
ende



---

### 🏆 Gewinn-Anzeige

wenn ich [Rot gewinnt v] empfange
wechsle zum Kostüm [Rot gewinnt v]
warte (3) Sekunden
ende

---

### Mögliche Erweiterungen

- 🏅 Punkte-System statt einfacher Sieg
- 🎵 Sound Effects bei Kollisionen
- 🌍 Mehrere Rennstrecken
- 💨 Speed-Boosts auf der Strecke
- 🤖 KI-Gegner statt lokalem Multiplayer

---

## 📄 Lizenz & Credits

Entwickelt von **Leon Wüste** für das Diesterweg-Stipendium 2026.

Dieses Projekt steht unter der MIT-Lizenz. Du darfst es frei nutzen, modifizieren und weitergeben – mit Nennung des Originalautors.

---

## 🔗 Links

- [Scratch Editor](https://scratch.mit.edu)
- [Scratch Dokumentation](https://scratch.mit.edu/info/faq)
- [Diesterweg-Stipendium](https://www.diesterweg-stipendium.de)

---

**Viel Spaß beim Spielen und Programmieren! 🎮✨**
