# Cadliner ASCII

Wandelt ein Bild in ASCII-Art um, die man mit dem Beschriftungsgerät **MAX Cadliner CD-750** Zeichen für Zeichen abschreibt – und hakt den Fortschritt über mehrere Tage ab.

Eine einzelne HTML-Datei, ohne Installation und ohne Internet: [`Cadliner_ASCII.html`](Cadliner_ASCII.html) herunterladen und im Browser (Chrome/Edge/Firefox) öffnen.

## Funktionen

- **Papier & Schrift wie am Gerät:** Papierformat, Ränder, Schrifthöhe (1,0–25,4 mm), Breite (50–200 %), Buchstabenabstand (1/10 h) und Zeilenabstand. Spalten/Zeilen werden daraus berechnet.
- **Nur Zeichen, die das Gerät kann:** Groß-/Kleinbuchstaben, Ziffern, Satzzeichen einzeln wählbar, eigene Zeichen ergänzbar, Anzahl der Zeichenarten begrenzbar. Die Tinten-Dichte jedes Zeichens bestimmt den Grauwert.
- **Tonwerte:** Helligkeit, Kontrast, Gamma, Schärfe, Hintergrund freistellen, Dithering, Autokontrast – mit Zurücksetzen-Button (Doppelklick setzt einzelne Regler zurück).
- **Schreibfeld 185 × 40 mm:** Das Bild wird in Geräte-Felder geteilt; die App sagt, wann das Gerät umgesetzt werden muss.
- **Mehrfarbig:** bis zu 8 Stifte. Pro Zelle wird die beste Kombination aus Stift *und* Zeichen gewählt. Farbvorschlag aus dem Bild, Pipette, Hinweis „Stift wechseln“, Filter „nur aktueller Stift“.
- **Abhaken:** Klick, Shift+Klick, ganze Zeile; Schreibleiste mit nächstem Zeichen, Position in mm und Leerschritten. Tastatur: Leertaste/Enter, Rücktaste, Strg+Enter, Strg+Z.
- **Speichern:** automatisch im Browser, zusätzlich als `.json`-Projektdatei (Strg+S) zum Sichern und Weitergeben.
- **Export:** 1:1-Druck, TXT (je Stift ein Abschnitt), SVG (eine Gruppe pro Stift – für Plotter).

## Hinweise zum CD-750

- Kein PC-Anschluss vorhanden (nur Netzteil und Schrift-Kassette). Automatisierung ginge nur per Umbau, z. B. Tastatur-Matrix per Mikrocontroller „drücken“ oder Schrittmotoren direkt mit GRBL ansteuern.
- Der Monitor-Modus puffert bis zu 200 Tastenanschläge – eine Zeile vortippen, prüfen, schreiben lassen.
- Neigung auf 90° lassen; bei mehreren Farben das Gerät beim Stiftwechsel nicht verschieben.
