- Linear durchgängiges Level, von A nach B
- Ein Level, das mit verschiedenen Skill-Kombis mind. 2x spielbar ist
- Aufbau: 2 Räume, 1 Brunnen, 1 Raum, Endboss
- Räume OHNE zurückgehen

- ==🔴Ursprünglich 3 Teile eines Levels: Swamp, kompletter Dungeon, Endboss ODER pro Seele wird es anders angehaucht, heißt man hat Seelen-Level im Swamp oder im Duengeon etc.==

# Gamesicht

- Character Fokussierung der Kamera
- Raum ist größer als Kamera-Blickfeld
- **Raumübergang & Aufbau**: visuelle Abgrenzung innerhalb begehbarer Struktur, aber gesamtes Level mit allen Raum-Szenen soll falls möglich bereits geladen sein 


![[Gameplay view Hades.jpg|536]]



![[Gameplay View Cult of the Lamb.png|548]]

# Setting - Moodboards

![[Moodboard Benita Charon.png]]

**Spezifisch Leveldesign:** 

![[Moodboard Level Design Swamp.png|700]]

+ Dunkler, nebeliger, düsterer, Lila-tinge, verfallene griechische Strukturen

# Ablauf des Games: Sequenzielle Reihenfolge

- Startmenü [[Screens#Startmenü]]
- Einführung in Lore/Story
- Seelenzuweisung in bereits interaktiver Umgebung
- Wahl der Oboli-Coins (auf 2 beschränkt) in [[Screens#Auswahlmenü Oboli]] 
- Betreten des Levels
- Kampf-Eintritt
- 3 Räume Kampf
- Lebensbrunnen 
- 2 Räume Kampf
- Endboss
- Ende des Levels
# Tutorial

- Erster kleiner Raum zur Einführung in [[Tutorial]]
- Angeleitet von [[Figuren#Der Tod]] aus Einführung in Lore

# Einführung in Lore/Story/Cutscene 

- BEVOR bzw WÄHREND Seelen-Zuweisung stattfindet
- Interaktion mit [[Figuren#Der Tod]] für Dialog und Eintauchen in die Lore
- Evtl. teils auch Szenisch stattfindend in [[Screens#Level-Auswahl]]
# Im Level: Raumaufteilung

## Übergänge zwischen Räumen

- Brücke + Torbögen
- Durch Nebel verschleiert  wenn man noch nicht durch kann
## Kampfraum

- Raum-Individualisierung: Bestehende Assets neu kombinieren
- ODER von Sumpf immer mehr steigern auf verfallene griechische Struktur
- Hindernisse, Abgrenzungen einbauen
- Gegner-Zusamenstellung, wie viele, Spawn-verhalten und [[Figuren#Gegnertypen]]
## Pauseraum: Lebensbrunnen

- Safe-Checkpoint im Level
- ==🔴Bei Mehr Räumen Überlegung: Evtl sogar nach jedem Raum, aber mit verschiedenen Belohnungen: Heilung, Level-Ups==  
- **Interaktion**: Rasten
	- Heilt Charakter
	- Füllt Heiltränke auf
	- Checkpoint für Respawns nach Tod: Speichert Spielstand
	- ==🔴Rogue-Like Level Ups von Seelen- und Obolus Skills==
- **Visueller Hinweis** auf Interaktion: Leuchtet, strategisch platziert

## ==🔴Bossfight==

- ==🔴Pantheon==

---
# Benötigte Environment Assets 

**Darauf achten:** 
- Origin der Game Assets zum auf Szene setzen an den Boden (Clipping)
	- Edit mode , Plane selection, Shift + S, 3d cursor to selected, Objekt Mode, Origin to 3d cursor
- Collision Shapes adden, Grundform des Objekts


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