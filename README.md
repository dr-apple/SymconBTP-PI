# SymconBTP PI Version

Diese Version ist eine minimal abgeänderte Version von traxanos ! Das original : https://www.symcon.de/forum/threads/28860-Bluetooth-Presence-Modul-%28Linux-Only%29

SymconBTP ist eine Erweiterung für die Heimautomatisierung IP Symcon. Diese Erweiterung stellt eine alternative zum gängigen Geofancing dar. Dabei dient das Bluetoothgeräte (meist das Mobiltelefon) als Erkennungsmerkmal. Wird beim Scan ein Gerät mit der hinterlegten MAC-Adresse gefunden, so wird der Status auf Anwesend gesetzt. Zusäzlich wird zum Status noch das Datum des Zustandwechsel sowie der Gerätename gespeichert.

## Einrichtung

Die Einrichtung erfolgt über Modulverwaltung von Symcon. Nach der Installation des Moduls sollte der Dienst neugestartet werden. Danach kann man pro Gerät eine Instanz vom Typ "Presence Device" anlegen.

## Einstellungen

* **MAC**  _Die MAC des Geräte_
* **Interval**  _In welchem Abstand soll nach dem Gerät gesucht werden_

## Voraussetzung

* R PI 
* Bluez (hcitool) 
Hier eine Anleitung: https://www.symcon.de/forum/threads/27730-Der-PI-ibeacon-mit-%C3%BCber-30-40m-Reichweite-perfekt-f%C3%BCr-Anwesenheitserkennung-%21?highlight=beacon

* Bluetooth Dongle

* ab Symcon Version 4


## Funktionen

	// Sucht nach dem Bluetoothdevice
	BTP_Scan($id);
	
