
# Betriebssysteme

---
## Anforderungen und Aufgaben

- Software, die zusammen mit der Hardware die Basis zum Betrieb d. IT-Systeme
- BS macht die Benutzung des Computers möglich
---

Bsp.
- Windows
- MacOS
- Linux
	- Ubuntu
---
# Aufgaben

---
## Dateiverwaltung
- Programme u. Daten müssen gespeichert werden, da Inhalte des Arbeitsspeichers verloren gehen bei Stromverlust
- Daten werden, in Form von Dateien gespeichert
- Die Logik der Dateiverwaltung wird in Form eines Dateisystems von Betriebssysteme zur Verfügung gestellt

---

## Speicherverwaltung
- ordnet Speicherbereiche dem aus. Prozessen zu
- gibt Speicher frei der nicht benötigt wird
- wenn nicht alle Programme Platz finden müssen Daten auf die Festplatte temporär ausgegliedert werden

---

## Prozessverwaltung
- Ressourcen (Betriebsmittel) des Computers werden zwischen allen laufenden Prozessen und Programmen aufgeteilt
- Das betrifft vor allem die Prozessorzeit

---

## Steuerung der Hardware
- Computersysteme sind modular aufgebaut und dessen Bestandteile austauschbar
- Hardwaresteuerung regelt mit Hilfe von Gerätetreibern den Zugriff auf die verschiedenen Geräte

---

## Ein- u. Ausgabesteuerung
- Betreibsysteme steuern die Zusammenarbeit der verschiedenen Ein- und Ausgabegeräte
  wie Tastatur u. Bildschirm
- auch die E|A Operationen mit Peripheriegeräten gehören dazu
---
## Bereitstellen von d. Benutzeroberfläche
- Benutzeroberfläche (GUI - Graphic User Interface) ist ein Spezialfall der E|A - Steuerung
- dient ausschließlich der Kommunikation mit dem Benutzer, um dessen Aufgaben zu erledigen

---

## Erteilung von Betriebssystemen
---
1. Anzahl gleichzeitig laufender Programme
	- Einzelprogrambetrieb (single-tasking)
	- Mehrprogrambetrieb (multi-tasking)
---
2. Anzahlgleichzeitig arbeitender Benutzer
	- Einzelbenutzerbetrieb (single user mode)
	- Mehrbenutzerbetrieb (multi user mode)
---
3. Anzahl verwendeter Prozessoren
	- Ein-Prozessor-Betriebssystem
	- Mehr-Prozessor-Betriebssystem
---
4. Betriebsart
	- Stapel-verarbeitung (Stack)
	- Dialoge-betrieb
	- Netzwerk-betrieb
	- Echtzeit-betrieb

---
## Architektur, Aufbau und Modelle
---
- Betriebssystem ist gegenüber Anwendungsprogrammen privilegiert beim Zugriff auf Betriebsmittel, wie Geräte und Prozessor
---
- Schallen-modell
	- Schnittstellen bilden Übergänge zwischen den Schichten
	- Zugriff von Anwendungen direkt auf die Hardware oder die Prozessverwaltung usw. sind ausgeschlossen.
	- Modell:
		- Hardware
		- Speicherverwaltung, Prozessverwaltung
		- Kernel (Systemdienste)
		- Anwendungen
---
- Schichten-modell
  (als Alternative)
	- Modell:
		- Prozessor, Speicher, Geräte
		- Kernel
		- Anwendungsprogramme

---
## Kernel

- stellt die Schnittstelle zu den Anwendungsprogrammen dar
- kontrolliert den Zugriff auf den Prozessor, Geräte und Speicher
- verteilt Betriebsmittel, wie z.B. Prozessorzeit auf die Anwendungsprogramme
---
#### Monolihtischer-Kernel
- Alle Programmteile laufen im privilegierten Kernelmodus
- daraus resultiert Umschaltzeiten zwischen den einzelnen Systemaufrufen
- Bei Änderungen eines Teils des Kernels muss er komplett neu kompiliert werden
---
#### Micro-Kernel
- verkleinerte Anzahl an Funktionen, die im Kernelmodus ausgeführt werden
- Kritische Bereiche werden kleiner und Übersichtlicher
	-> System wird stabiler
- Durch Wechsel zwischen Benutzer- und Kernelmodus wird das System langsamer
---
#### Hybrid-Kernel
- ist nicht so Fehler anfällig wie der monolithische-Kernel
- nicht alle Treiber laufen im privilegierten Modus
- bei einem Fehler stürzt nicht das ganze System ab
- aber es sind auch nicht so viele Kontextwechsel (Benutzer, Kernel) nötig wie beim Mikro-Kernel
	-> Geschwindigkeit höher als beim Mikro-Kernel

---

| Anwender            | Anwendungen                                | Anwendungen                                                                 | Anwendungen                           |
| ------------------- | ------------------------------------------ | --------------------------------------------------------------------------- | ------------------------------------- |
| Betriebs-<br>system | Systemaufrufe                              |                                                                             | Dateisystem<br>Server-<br>Prozesse    |
| - \|\| -            | Memory Manager<br>Dateisystem<br>Scheduler | Server-<br>Prozesse<br>System-<br>Prozesse<br>Dateisystem<br>Geräte Treiber | System-<br>Prozesse<br>Geräte Treiber |
| - \|\| -            | Geräte Treiber                             | Memory Manager<br>Scheduler                                                 | Memory Manager<br>Scheduler           |
| - \|\| -            | Hardware                                   | Hardware                                                                    | Hardware                              |
| - \|\| -            | Monolithischer<br>Kernel                   | Mikro<br>Kernel                                                             | Hybrid<br>Kernel                      |
