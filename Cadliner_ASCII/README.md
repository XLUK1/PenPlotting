# Cadliner ASCII

Wandelt ein Bild in ASCII-Art um, die man mit dem Beschriftungsgerät **MAX Cadliner CD-750** Zeichen für Zeichen abschreibt – und hakt den Fortschritt über mehrere Tage ab.

Zweiter Modus **„Kreuzstich / Pixel-Raster“**: dasselbe Bild als Farbraster mit Symbolen – für Kreuzstich, Bügelperlen, Karopapier, Mosaik oder Strickmuster.

Eine einzelne HTML-Datei, ohne Installation und ohne Internet: [`Cadliner_ASCII.html`](Cadliner_ASCII.html) herunterladen und im Browser (Chrome/Edge/Firefox) öffnen.

## Funktionen

- **Papier & Schrift wie am Gerät:** Papierformat, Ränder, Schrifthöhe (1,0–25,4 mm), Breite (50–200 %), Buchstabenabstand (1/10 h) und Zeilenabstand. Spalten/Zeilen werden daraus berechnet.
- **Monospace wie am Gerät:** Standard-Zeichenabstand = Schrifthöhe (Mitte bis Mitte, laut Anleitung) – feste Spalten. Alternativ Abstand über LETTER SPACE. Vorschau und Tinten-Dichte mit DIN-ähnlicher Engschrift: Google Font „Barlow Condensed“ (online), offline Ersatz Bahnschrift Condensed / Arial Narrow.
- **Hell auf dunkel:** Untergrund „Dunkel – helle Stifte“ mit frei wählbarer Papier- und Stiftfarbe; helle Bildstellen werden dicht beschrieben. Auch im Mehrfarbmodus (Mischung mit der echten Papierfarbe, Stiftvorschlag mit hellem Grundstift).
- **Nur Zeichen, die das Gerät kann:** Groß-/Kleinbuchstaben, Ziffern, Satzzeichen einzeln wählbar, eigene Zeichen ergänzbar, Anzahl der Zeichenarten begrenzbar. Die Tinten-Dichte jedes Zeichens bestimmt den Grauwert.
- **Tonwerte:** Helligkeit, Kontrast, Gamma, Schärfe, Hintergrund freistellen, Dithering, Autokontrast – mit Zurücksetzen-Button (Doppelklick setzt einzelne Regler zurück).
- **Schreibfeld 185 × 40 mm:** Das Bild wird in Geräte-Felder geteilt; die App sagt, wann das Gerät umgesetzt werden muss.
- **Mehrfarbig:** bis zu 8 Stifte. Pro Zelle wird die beste Kombination aus Stift *und* Zeichen gewählt. Farbvorschlag aus dem Bild, Pipette, Hinweis „Stift wechseln“, Filter „nur aktueller Stift“.
- **Abhaken:** Klick, Shift+Klick, ganze Zeile; Schreibleiste mit nächstem Zeichen, Position in mm und Leerschritten. Tastatur: Leertaste/Enter, Rücktaste, Strg+Enter, Strg+Z.
- **Speichern:** automatisch im Browser, zusätzlich als `.json`-Projektdatei (Strg+S) zum Sichern und Weitergeben.
- **Export:** 1:1-Druck, TXT (je Stift ein Abschnitt), SVG (eine Gruppe pro Stift – für Plotter).

## Modus „Kreuzstich / Pixel-Raster“

- **Raster & Stoff:** Aida 11/14/16/18 ct, Leinen 28/32 ct über 2 Fäden, Bügelperlen (5 / 2,6 mm), Karopapier oder eigene Kästchengröße. Breite in Kästchen, Höhe aus dem Bildformat; fertige Größe und Stoffzuschnitt (mit Zugabe) werden angezeigt.
- **Garn-Palette:** 2–40 Farben, Vorschlag aus dem Bild (k-Means im Lab-Farbraum), Pipette, Name/Garn-Nummer frei (z. B. „DMC 310“). Jede Farbe bekommt ein eindeutiges Symbol.
- **DMC-Garne:** 489 DMC-Farben eingebaut (Mouliné, inkl. Blanc/Ecru/B5200 und 1–35). Vorschlag direkt als DMC-Garne ohne doppelte Nummern, DMC-Nummer eintippen übernimmt die Farbe, „Alle auf DMC runden“. Farbwerte aus [JuliaSzulc/flossverter](https://github.com/JuliaSzulc/flossverter) (abgeglichen mit einer zweiten Liste, DMC 699 korrigiert) – Bildschirm-Näherungen.
- **Saubere Muster:** Hintergrund (Stofffarbe) frei lassen, Einzelstiche entfernen, Dithering optional. Eigene Tonwert-Standards ohne Schärfen und Raster.
- **Abhaken:** Farbe für Farbe, Block für Block oder Zeile für Zeile; Anzeige Farbe + Symbol, nur Symbole oder nur Farbe; Schreibleiste zeigt „n Stiche am Stück“; Fortschritt pro Farbe.
- **Muster drucken:** A4-Seiten mit Symbolen, 10er-Linien und Spalten-/Zeilennummern, farbig oder schwarz-weiß, Kästchengröße einstellbar; letzte Seite mit Übersicht, Seitenaufteilung und Legende (Stiche je Farbe).
- **Export:** SVG als Pixelbild in Originalgröße (ein Pfad pro Farbe), TXT als Symbolraster mit Legende.

## Hinweise zum CD-750

- Kein PC-Anschluss vorhanden (nur Netzteil und Schrift-Kassette). Automatisierung ginge nur per Umbau, z. B. Tastatur-Matrix per Mikrocontroller „drücken“ oder Schrittmotoren direkt mit GRBL ansteuern.
- Der Monitor-Modus puffert bis zu 200 Tastenanschläge – eine Zeile vortippen, prüfen, schreiben lassen.
- Neigung auf 90° lassen; bei mehreren Farben das Gerät beim Stiftwechsel nicht verschieben.
