# Blockwelt V145 – Safari-Startfehler behoben

## Konkrete Ursache

In V144 waren zwei gleichnamige Funktionen `pawPart` im selben JavaScript-Modul deklariert, obwohl sie unterschiedliche Aufgaben erfüllen. Safari verweigerte deshalb schon das Einlesen des Moduls mit: `Cannot declare a function that shadows a let/const/class/function variable pawPart`.

V145 verwendet stattdessen `createPawPortalPart` für das Eingangstor und `createPawHQPart` für bewegliche Bauteile der PAW-Zentrale. Beide Funktionen und alle ihre Aufrufe wurden getrennt und geprüft. Sämtliche relevanten Dateireferenzen wurden auf V145 gesetzt.

## Installation auf GitHub

1. Repository und falls möglich den Spielstand sichern.
2. Das ZIP entpacken.
3. Diese fünf Dateien im **Hauptverzeichnis** ersetzen: `index.html`, `game.js`, `styles.css`, `nachtrabe.js`, `paw-lookout-3d.glb`. Auch `README.md` aktualisieren.
4. Änderungen auf `main` übernehmen; Force Push aus.
5. In GitHub Pages den Repository-Pfad mit `?v=145` aufrufen. Nicht die Safari-Website-Daten löschen.

## Inhalt

- Integrierte PAW-Zentrale als eigenständig erstelltes GLB-3D-Modell; kein offizielles PAW-Patrol-Modell.
- Bestehende Spielwelt mit Schloss Nachtrabe und den vorgesehenen PAW-Spielbereichen.
- Safari-Fehlerdiagnose bleibt erhalten.

## Prüfgrenzen

JavaScript-Syntax, doppelte Funktionsnamen, referenzierte lokale Dateien, GLB-Lesbarkeit und ZIP-Struktur sind geprüft. Ein vollständig erfolgreicher Spielstart auf deinem iPhone ist damit nicht bewiesen.
