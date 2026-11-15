# Blockwelt V143 – Neue 3D-Modell-Zentrale

Dieses Paket ist fuer dein neues Repository gedacht.
Die bisherige Zentrale wird durch die neue 3D-Modell-Zentrale ersetzt.

Enthaltene Dateien:
- index.html
- styles.css
- game.js
- nachtrabe.js
- paw-lookout-3d.glb

Installation auf GitHub:
1. ZIP entpacken.
2. Alle 6 Dateien direkt ins Hauptverzeichnis des Repositorys hochladen.
3. Keine Unterordner anlegen.
4. Danach GitHub Pages auf main / (root) stellen.

# BLOCKWELT V143 – VOLLSTÄNDIGES ERSATZPAKET

Dies ist ein sauberer SPIELSTAND aus V142 mit dem begehbaren, selbst erstellten
PAW-Lookout als echtem GLB-3D-Modell. Keine Zusatzdateien vom Weißen Haus oder
von Burg Hohenzollern. Alle fünf Spieldateien liegen DIREKT im ZIP-Hauptordner.

## Was korrigiert wurde
- Kein automatisches Überschreiben der mitgelieferten 3D-Zentrale mehr durch
  alte, lokal gespeicherte GLB-Importe (IndexedDB bleibt unangetastet).
- Ein sichtbarer GLB-Ladestatus im Menü zeigt, ob die Zentrale wirklich lädt.
- Meldung bei nicht startendem Spiel statt dauerhaft hängendem Ladebildschirm.
- Alle Versions- und Cache-Parameter von V142 auf V143.
- Fünf benötigte Dateien ohne fremde Modelle oder zusätzliche Ordner.

## So wird die Version vollständig ersetzt (Working Copy / GitHub)
1. Im bisherigen Spiel unter "Welt sichern" die persönliche Welt als JSON
   exportieren. Danach das GitHub-Repository zur Sicherheit ebenfalls sichern.
2. Im Repository HeimHafen/Blockwelt im gewünschten Branch ALLE alten
   WEB-SPIELDATEIEN im Hauptverzeichnis entfernen, die NICHT zur untenstehenden
   Fünferliste gehören. Alte Website-Dateien bleiben andernfalls bestehen.
   WICHTIG: Vorher prüfen, ob darin Inhalte anderer Projekte stecken.
3. ZIP in der Dateien-App entpacken und die FÜNF Spieldateien einzeln in das
   Hauptverzeichnis des Repositories kopieren; NICHT das ZIP selbst hochladen
   und KEINEN Unterordner Blockwelt_V143_KOMPLETT_ERSETZEN erstellen.
4. Im Repository-Hauptverzeichnis müssen exakt diese fünf Web-Spieldateien
   vorhanden sein: index.html, styles.css, game.js, nachtrabe.js,
   paw-lookout-3d.glb. Eine vorhandene .nojekyll oder CNAME-Datei, falls nötig,
   darf zusätzlich erhalten bleiben.
5. Git committen / pushen (Source: refs/heads/main; Remote: refs/heads/main;
   Force Push: AUS). Für eine sichere Vorabprüfung zunächst Testbranch nutzen.
6. https://heimhafen.github.io/Blockwelt/?v=143 im Safari-Browser laden.
   Oben muss V143 stehen. Menü > Welt & Grafik zeigt unter dem GLB-Import
   "3D-Modell: Geladen – begehbare Zentrale ist aktiv".
7. Bei Bedarf die vorher gesicherte JSON-Welt importieren. Nicht auf
   "Welt neu anfangen" tippen. Keine Safari-Website-Daten löschen.

## Diagnose, falls V143 immer noch nicht startet
- Noch V142/V140 oben? Die aktualisierte index.html wurde nicht geladen,
  der Cache ist noch alt oder du bist auf einem anderen Branch.
- GLB-Status "FEHLT"? Die Datei paw-lookout-3d.glb muss mit exakt diesem Namen
  direkt neben index.html und game.js liegen (Groß-/Kleinschreibung zählt).
- Bildschirm meldet Modulfehler? Das Spiel lädt Three.js 0.187.0 über jsDelivr;
  eine Netzwerksperre oder fehlende Internetverbindung verhindert den Start.
- Weitere alte Gebäudeteile? Persönliche Browser-Bauänderungen können erhalten
  bleiben; das Ersetzen der Repository-Dateien löscht gespeicherte Blöcke nicht.

WICHTIG: Die ZIP-Datei verändert dein GitHub-Repository nicht automatisch.
Sie ist ein VOLLSTÄNDIGES Ersatzpaket, keine serverseitige Aktualisierung.
Diese Rekonstruktion ist keine offizielle Original-GLB von PAW Patrol.

PRÜFSTAND: Dateipfade, alle fünf Dateien, glTF-Struktur und JavaScript-Syntax
geprüft; eine vollständige Laufprüfung im echten iPhone-Safari konnte hier
nicht durchgeführt werden. Bitte zunächst als Testversion betrachten.
