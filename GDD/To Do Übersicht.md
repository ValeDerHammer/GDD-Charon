✅Erledigt
➡Aktuelle Aufgabe

# Übersicht 

**ZEIT BIS ZUM 14. DEZEMBER**
- Gamenight am 12. Dezember: Leute spielen lassen fürs Balancing

**Fokus: Bindung + Skill-Sets**

- **WAS ist das technische Ziel:** 1 Level, das mind. 2x mit verschiedenen Skill-Kombis spielbar sein soll (insg. 4 Skills festgelegt)
- **WAS ist der Unique Selling Point:** Kampf mit Seele -> BINDUNG! + Durch Oboli werden verschiedene Seelen-Fähigkeiten kombinierbar pro Level 
- **WAS ist die Einbettung in Lore:** Charon hilft struggelnden Seelen beim Übergang ins Totenreich, side-along Combat-basiert + sehr leichte Story-Aspekte

---
## Person je Thema

Tobi: Level-Laden, Skillsystem
Benita: Level Design + Environment
Fynn: Combat (HP-System, Gegner KI)
Vale: Figuren 
Fabi: Menüdesign + Implementierung

------------------------------------------------------------------------------

Vale: 
- Playable Character Design + Mesh
- Playable Character Animationen
- 

Fynn: 
- Dash 
- Schadens- & HP-System, inkl. Gegner Angriff
- Interaktions Mechanic
- Gegner KI 
- Projekt Refactoren (Übersichtlicher, Kommentare)


Tobi: 
- Szenen-Wechseln
- Laden von Levelumgebung und Gegnern (Spawnobjekt) + Benita
- Skill System (Kombi Fynn)
- Speicherstände

Benita: 
- Level Skizze Design 
- Level Assets
- Level Aufbau
- Bindungssystem
- Story-Einführung

Fabi: 
- Startmenü (Spiel starten, Einstellungen, Spiel Verlassen) ansehnlich + klickbar machen
- Gesamte Menüführung und Game-Overlay


---
# Figuren und Assets

## Gegner

Zu Jedem Gegner gehört: Mesh, Textur, Riggen, 1 Angriff-Animation, 1 kurze WirdGehitted-Animation (Zurückweichen)
- Gegner Cauldron
- Gegner Geist Hand
- Gegner 3
- Gegner Skelett (Mesh steht schon) + Animation
- Gegner Endboss: Gitterbauch 

## Charon + Assets

- Character Charon: Mesh, Textur, Rigg, Animationen
	- Accessorie-Assets: Mesh und Textur
		- Seele
		- Schwebende Laterne mit Seele als eigene visuelle Entität
			- Animation: ZWEI verschiedene Seelen-Angriffe 
				- Boomerang + Enterhaken
			- Animation: Seele geht in Laterne rein + Seele geht aus Laterne raus
		- Hut
		- Mantel
		- Schwert
		- Heiltrank Mesh/png
	- Animationen: Heiltrank, LeichterKampf 1, SchwererKampf 1, Laufen, Dash, BrunnenInteraktion
	- Animation: Schwert leuchtet/brennt bei aktiver Bindung

- Asset Obolus 
	- Mesh 
	- // Erhalt-Animation
	- Animationen: ZWEI verschiedene Obolus-Angriffe (farblich getrennt zu Seelen)
		- Seelenbombe und Sound-Druckwelle

- 2x Obolus, 2x Seele = insg. 4 Skills designen und animieren

// - Animation Combat Bindungs-Kügelchen + Magnet-Effekt

------------------------
# Balancing 

- Combat Pacing
	- Laufgeschwindigkeit
	- Angriffspatterns
- Schaden Leben Ausdauer Bindung
- Belohnung, Fortschritt, Strafe

------------
# Code

- **Generelles**
	- Szenen-Wechseln
	- Laden von Levelumgebung und Gegnern (Spawnobjekt)
	- Speicherstände
	- Schadens- & HP-System, inkl. Gegner Angriff

- **Player Character:** 
	- Charakter WASD Kontrolle (gut soweit, Fynn)
	- Tasten und Funktion
		- Dash Mechanic überarbeiten
		- Heilen 
		- Skillsystem mit F1 und F2 (je nach Oboli-Ausrüstung andere Animation + Schaden)
			- 4 Seelen/Obolus Skills Implementieren: Animation verbinden + Schaden verbinden
				- Skill 1
				- Skill 2
				- Skill 3
				- Skill 4 
		- Interaktions Mechanic mit generellen Objekten (Brunnen)
	- Zielsystem (Angreifen wohin schauen)
	- Bindungssystem 

- **Gegner KI**
	- Gegner Pathfinding (okay soweit, Fynn)
	- Gegner Anpassung an Spielverhalten bzw. Art der Gegner 

------------------
# Menüs & Screens

- Schriftarten: Titel, Infotext, 2te kleinere Überschrift für bsp. Seelen-/Skill-Namen
	- Startmenü (Spiel starten, Einstellungen, Spiel Verlassen)
	- Einführung in Lore/Story/Cutscene vor Seelen-Wahl
	- Seelen/Level Auswahl (später: Rumlaufen Interaktion)
	- Auswahlmenü für Oboli (Umsetzung mby per Drag & Drop)
	- Loading-Bar
	- Im Level: 
		- ESC Pausenmenü geteilt in Technisch (Weiter spielen, Einstellungen, Verlassen) 
		und Level-Stats (Kurzbeschr Eigenschaften Seele + Obolus)
		- Todes-Screen 
		- Win Screen (Erhalt von Obolus, Dank der Seele)
		- Generelles Game-Overlay: Sichtbare Healthbar, Bindung (füllt sich / sinkt radikal auf 0), Ausdauer, 2 Skill Cooldowns (nur visuell, ohne zahlen)
	
	- Einstellungen: Grafik/Anzeige, Gesamtlautstärke + Sound + Musik-Lautstärke, Steuern (Custom Tastenbelegung), Blickrichtung Spieler Rotation to Mouse/Laufsteuerung änderbar

Einstellungen umsetzen
	- Custom Tastenbelegung 
	- Gesamtlautstärke
	- Sound- und Musik- Lautstärke

--------------------------------------------------------------------------

# Level Design + Environment

- Mit Fabi: Beginn des Spiels: Erhalt der Seele besprechen
- Soundentscheidungen
- Musikentscheidungen

- Level Skizze visuell: Anfangs nur 3 Räume designen
- Level Planung
	- Pro Kampf-Raum von Sumpf immer mehr steigern auf verfallene griechische Struktur

- **Environment Assets erstellen:** 
	- Boden (+ Textur?)
	- Sumpf-Bäume
		- Lianen
	- Gefallene Bäume / Äste 
	- Shrubs
	- Wasser
	
	- Glühwürmchen
	- Nebel
	
	- Ruinen
	- Mauer-Ruinen
	- Torbogen-Durchgang
		- Lianen, Moos
	- Brücke
	- Lebensbrunnen
	- Kerzen
	 - ~~Verfallene Brunnen~~

## Story-Aspekte

- WIE vermitteln?
- Zu Beginn Dialog mit dem Tod? Charakter Design - wie stellen wir ihn dar?
- Ganz kleiner Dialog - Seele Charon
- Seelen Auswahl + Einführung, Story, Tod, Lore vermitteln

