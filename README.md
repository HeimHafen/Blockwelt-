# BLOCKWELT V146 – PAW Lookout 3D-Testversion

Eigenständig erstellte Rekonstruktion des klassischen PAW-Patrol-Aussichtsturms. **Kein offizielles Original-Asset, keine behauptete 1:1-Lizenzmodellierung.** Die Geometrie ist eine echte glTF/GLB-Dreiecksmeshdatei, kein gestapeltes Voxelgebäude.

## Ziel und aktuelle Umsetzung

- **Alt entfernt:** Die ehemalige, automatisch aus Gras-/Stein-/Glasblöcken generierte PAW-Zentrale samt seitlicher Block-Garage wird in `buildPawColumn()` nicht mehr erzeugt. Nur der vorhandene Portalweg bleibt als Terrain.
- **Neu:** Ein einheitliches GLB mit rundem Sockel, weißem verjüngtem Turm, rot gedeckter Panorama-Etage, gelbem Drehperiskop, silbergrauer offener Spiralrutsche, durchsichtigen Scheiben, Geländern, 3D-Wappen, Leuchten, Werkzeug-/Garagenbereich, Umkleideraum, Einsatztisch, Mission-Monitor, sechs runden Hundehäuschen und einem Rettungsfahrzeug-Vorplatz.
- **Funktionsstand:** Fahrstuhl mit drei Halten (Eingang, Umkleideraum, Leitstelle); Rutsche, Ryders Stange, Ein-/Ausgangstüren, drehbares Periskop, wechselnde Missionen, Garagen-Wartungsaktion, Auswahl von Ausrüstung, sechs per Joystick steuerbare stilisierte Einsatzfahrzeuge.
- **Rückfallmöglichkeit:** Die vorherige V145 bleibt unverändert; nimm eine Sicherung deines Spiels und deines Repositorys vor.

## Das Zip wird ohne Mischversionen installiert

Alle sechs Dateien in den **Hauptordner** von `HeimHafen/Blockwelt` hochladen und die vorhandenen gleichnamigen Dateien ersetzen:

1. `index.html`
2. `styles.css`
3. `game.js`
4. `nachtrabe.js`
5. `paw-lookout-3d.glb`
6. `README.md`

Auf `main` committen und GitHub Pages mit Branch `main` / `/(root)` betreiben. Danach die Seitenadresse mit `?v=146` laden. Keine Unterordner hochladen, nicht die ZIP-Datei selbst hochladen. Ältere separate Modell- und Projektdateien bleiben nur dann im Repository, wenn du sie dort ausdrücklich selbst belässt; das ZIP kann fremde Dateien auf GitHub nicht automatisch löschen.

**Vorher im Spiel:** Menü → `Welt sichern` (JSON exportieren). Safari-Website-Daten nicht löschen, keine Spielstands-Rücksetzung durchführen.

### Working Copy
- Commit-Zusammenfassung: `Blockwelt V146 – bisherige Blockzentrale durch modellierte GLB-Lookout ersetzen`
- Detaillierte Informationen: `Alten Voxel-Turm und Block-Garage entfernt; neues GLB mit Panorama, Rutsche, 3-Etagen-Fahrstuhl und sechs Hundehäuschen; Spielcode, Geometrie und Kollisionsregion angepasst.`
- Source: `refs/heads/main`
- Vorhandene oder neue Remote-Referenz: `refs/heads/main`
- Force Push: **Aus**

## Prüfstand / Grenzen

- `node --check` für beide JS-Dateien bestanden.
- Die GLB-Geometrie mit Trimesh wieder eingelesen und eine *tatsächliche* Modellansicht daraus gerendert. Keine KI-Konzeptgrafik als Live-Screenshot ausgegeben.
- Die alte `buildPawColumn`-Blockstruktur wurde entfernt; Modell und Rutschenbahn / Fahrstuhletagen wurden geometrisch abgeglichen.
- Browser-Test auf dem iPhone / vollständiger Echtzeit-WebGL- und Kollisionstest **noch nicht durchgeführt**. Bitte zuerst im Testbranch veröffentlichen und vor produktiver Nutzung auf dem Gerät prüfen.
- **Kein perfektes offizielles 1:1-Modell.** Exakte Serieninnenräume, Marken-Assets, reife Fahrphysik, Kameraführung, Animationen und publikationsgeeignete Lizenzklärung bleiben gesonderte Arbeitsschritte. Dies ist ein hochwertigerer geometrischer Neubau als Teststand, keine finale Abnahme.
- Three.js wird online von einem CDN geladen; beim allerersten Start ist ein Internetzugang erforderlich.

## Testreihenfolge

1. Der Kopfbereich zeigt V146, keine Startdiagnose.
2. Die neue Zentrale steht **allein**, ohne durchragende Blöcke und seitliche Alt-Garage.
3. Vom Vorplatz durch den Eingang; innen freie Wege prüfen.
4. Den Fahrstuhl nacheinander zu Umkleideraum und Leitstelle benutzen; später zurück zum Erdgeschoss.
5. In der Leitstelle Mission wechseln, Periskop bewegen, Ryder-Stange und Rutsche testen.
6. Hundehäuschen erreichen und die Einsatzfahrzeuge fahren / verlassen.
7. Menüs, Bauwerkzeug, Speicherstand und andere bereits vorhandene Blockweltbereiche gegenprüfen.
