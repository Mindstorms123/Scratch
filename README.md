# Scratch

<img width="1783" height="1157" alt="grafik" src="https://github.com/user-attachments/assets/facfab1d-afa7-484f-ad1a-5e85955aa2ab" />

Dieses Projekt ist ein einfaches 2-Spieler-Rennspiel für Scratch, entwickelt für eine Schulung im Rahmen des Diesterweg-Stipendiums (5. Klasse). Zwei Spieler rasen auf einer runden Strecke gegeneinander – wer zuerst die Flagge berührt, gewinnt!

Features
2-Spieler-Steuerung: Spieler 1 (rotes Auto): Pfeiltasten | Spieler 2 (gelbes Auto): WASD

Gleichzeitiges Lenken + Fahren: Vor-/rückwärts und Drehen parallel möglich

Timer: Laufende Stoppuhr oben links

Gewinn-Bedingung: Berührung der Zielflagge zeigt Siegesbild

Sprites: Custom Rennwagen (rot/gelb) und Strecke im Pixel-Stil

Steuerung
Spieler	Vorwärts	Rückwärts	Links	Rechts
Rot (Pfeile)	↑	↓	←	→
Gelb (WASD)	W	S	A	D
Installation & Start
Gehe zu scratch.mit.edu und erstelle ein neues Projekt

Lade die Assets hoch:

Rennstrecke: Screenshot – als Hintergrund

Rotes Auto: Sprite

Gelbes Auto: Sprite

Gewinn-Bilder: Rot/Gelb gewinnt

Kopiere die Scripts aus den Screenshots oder unten

Klicke grüne Flagge – los geht's!

Scripts (wichtigste Blöcke)
Für beide Autos (anpassen für Tasten):
text
wenn grüne Flagge
  gehe zu Startposition
  für immer:
    [Tasten-Checks parallel]
    wenn Flagge → Gewinn-Bild + stoppe
Timer-Sprite:

text
wenn grüne Flagge → stoppuhr zurücksetzen
für immer → sage (runde stoppuhr)
Assets (hier generiert)
Rennstrecke ohne Timer/Autos

Rotes Auto (Pixel)

Gelbes Lamborghini-Auto

Gelb gewinnt!

Rot gewinnt!

Für Lehrer/Schulung
Dauer: 45 Min (Setup 10 Min, Bauen 20 Min, Remix 15 Min)

Lernziele: Schleifen, Bedingungen, Variablen, Kollisionen

Erweiterungen: Bestzeiten speichern, Hindernisse, Power-Ups

Lizenz: CC-BY-SA (freie Nutzung mit Quellenangabe)

Entwickelt von Leon Wüste für Diesterweg-Stipendium 2026.
