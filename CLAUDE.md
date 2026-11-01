# Mystic Adventures – Hinweise für Claude

- Das Spiel steckt komplett in `index.html` (eine Datei, Mobil-Web-App).
- **Jede Änderung am Spiel bekommt einen Eintrag in „Was ist neu?“**: oben im Array `NEWS` (in `index.html`, Abschnitt „Was ist neu (Update-Hinweise)“) einen neuen Eintrag mit nächsthöherer `v`-Nummer, Datum (`d`, z. B. '31. Oktober'), kurzem Titel (`t`) und 2–5 kurzen Stichpunkten (`l`) auf Deutsch, in einfacher Sprache für Spieler.
- Kommunikation mit dem Nutzer auf Deutsch.
- Grafik: Figuren (Held, Nekro-Bilder, Monster, Geister-Diener) laufen über PixiJS/WebGL (`pixi.min.js`, Objekt `GLR`): `drawImage`-Aufrufe auf die Bodenebene werden während `GLR.cap` abgefangen und als Pixi-Sprites gezeichnet. Hintergrund liegt als Bild im Element `#bgl`, Boden-Vektoren auf `#cv`, Effekte/Schrift auf `#ovc`. Schalter in ⚙ „Grafik-Engine“ (Klassisch = alter 2D-Weg).
- Hilfen zur Fehlersuche: ⚙ → 🛠 Diagnose, Sicher-Modus `?safe=1`, Testschalter `?alt=n|g|m|k|alle`. Spiel-Adresse: `ma-alx.github.io/Mystic/` (großes M).
