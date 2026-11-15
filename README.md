# BLOCKWELT – NEUSTART (V137)

Dies ist der originale, gesicherte Blockwelt-Spielcode aus `Blockwelt-main.zip` (V137).
Keine Dateien oder Modelle des Weißen Hauses. Keine nachträglich eingemischten V138–V143-Tests.

## Was ist enthalten?

- `index.html` – Spieleinstieg
- `styles.css` – Gestaltung und Bedienoberfläche
- `game.js` – Spiel und Weltlogik
- `nachtrabe.js` – Architektur von Schloss Nachtrabe

Die Welt enthält neben Schloss Nachtrabe auch ihre originalen weiteren Spielbereiche, unter anderem den älteren PAW-Patrol-Bereich. Es handelt sich **nicht** um die später geplante originale, voll funktionale GLB-Zentrale.

## Installation in GitHub

1. In GitHub unter Owner `HeimHafen` ein neues Repository `Blockwelt` erstellen; **Public** wählen.
2. Am besten **kein README initialisieren**, da dieses Paket eine eigene README mitbringt.
3. Dieses ZIP auf dem iPhone entpacken. **Die fünf enthaltenen Dateien** direkt im Hauptverzeichnis des Repositories hochladen – nicht den ZIP-Ordner und nicht das ZIP als Datei.
4. Commit auf `main` durchführen.
5. Einstellungen → Pages → Build and deployment: **Deploy from a branch**, Branch **main**, Ordner **/(root)**; speichern.
6. Website unter `https://heimhafen.github.io/Blockwelt/` öffnen.
7. Spielbetrieb auf iPhone testen: Menü, Bewegung, Schloss, Portale, Speichern, Laden.

Hinweis: Falls GitHub das alte Repository nicht sofort wieder unter `Blockwelt` zulässt, nimm `Blockwelt-Neustart` und passe den Pages-Link entsprechend an.

## Wichtige Datensicherheit

Der persönliche Spielstand war im Browser gespeichert, nicht im GitHub-Repository. Ein gelöschtes Repository enthält keine Sicherung der privaten Spielstände. Safari-Sitedaten nicht löschen; bei vorhandenem JSON-Export im Spielmenü `Welt laden` nutzen.

## Technische Grenzen

Die lokalen vier Spieldateien und JavaScript-Syntax wurden geprüft. Die 3D-Bibliothek Three.js wird über das Internet geladen. Dies ist ein wiederhergestellter, noch nicht auf deinem iPhone erneut getesteter Basisstand.

## Working Copy

- Zusammenfassung: `Blockwelt Neustart – V137 Schloss Nachtrabe wiederhergestellt`
- Detaillierte Informationen: `Saubere Wiederherstellung des gesicherten Blockwelt-Codes ohne fremde 3D-Projektdateien; HTML-Versionsanzeige korrigiert.`
- Source-Referenz: `refs/heads/main`
- Vorhandene oder neue Remote-Referenz: `refs/heads/main`
- Force Push: **Aus**
