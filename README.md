# Blockwelt V144 – reparierter Start und genaue Fehlerdiagnose

Dieses Paket ist für das neu angelegte Repository bestimmt. Es enthält die vollständigen 5 Spiel-Dateien und die README.

Dateien: index.html, styles.css, game.js, nachtrabe.js, paw-lookout-3d.glb, README.md.

## Installation (GitHub über iPhone)
1. Die bisherige Blockwelt sichern, falls im Menü verfügbar. Das Repository zusätzlich als ZIP speichern.
2. Dieses Paket entpacken.
3. Die fünf Spieldateien direkt in das Repository-Hauptverzeichnis hochladen und bestehende Dateien ersetzen. README.md zusätzlich hochladen.
4. GitHub Pages: Settings → Pages → Deploy from branch → main / (root).
5. Nach Veröffentlichung `?test=144` an die korrekte GitHub-Pages-URL anhängen. Oben muss **V144** stehen.

## Was anders ist
- Alle importierten Dateien haben einen einheitlichen Cache-Parameter 144.
- Prüft vor dem Spielstart auf GitHub Pages, ob die vier benötigten Ressourcen ausgeliefert werden.
- Prüft die externen Three.js-Bibliotheken. Bei Ausfall von jsDelivr wird unpkg ausprobiert.
- Zeigt bei einem Fehler **den tatsächlichen Modul- oder JavaScript-Fehler**, statt pauschal unvollständige Uploads zu behaupten.
- Die GLB-Datei ist eine eigene 3D-Rekonstruktion, keine offizielle Originaldatei aus PAW Patrol.
- Browser-Speicherstände werden nicht verändert.

## Einschränkung
Ein JavaScript-Syntaxcheck ersetzt keinen Laufzeittest auf dem iPhone. Ein Fehler kann erst im Browser sichtbar werden. In diesem Fall bitte die detaillierte Startdiagnose fotografieren.
