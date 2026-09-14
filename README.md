# Hochzeitsseite – Sprachauswahl (heller Prototyp)

Statischer Prototyp der Sprachauswahl mit dem Wappen. Löwe und Adler „liegen sich in den Armen"; heller, warmer Hintergrund. Reine HTML/CSS/JS-Seite, kein Backend – läuft direkt auf GitHub Pages.

## Dateien
- `index.html` – Sprachauswahl (linke Hälfte = Löwe = Nederlands, rechte Hälfte = Adler = Deutsch)
- `lorem_de.html` / `lorem_nl.html` – Platzhalter-Zielseiten (später durch die echten Seiten ersetzen)
- `assets/` – transparente Wappen-Teile: `lion.png`, `eagle.png`

## Interaktion
- **Desktop:** Maus über die linke/rechte Hälfte → die jeweils andere Figur wird grau; Klick führt weiter.
- **Handy:** Erster Tipp wählt (andere Figur wird grau) und blendet „Ga verder / Weiter" ein, zweiter Tipp führt weiter.

Die Zuordnung: linke Bildhälfte = Nederlands, rechte Bildhälfte = Deutsch. Löwe und Adler dürfen sich in der Mitte überlappen – die Auswahl hängt an der Bildhälfte, nicht am genauen Umriss.

## Auf GitHub Pages veröffentlichen
1. Neues Repository anlegen (z. B. `hochzeit`).
2. Inhalt dieses Ordners hochladen (`index.html` & Co. im Wurzelverzeichnis, `assets/` als Unterordner).
3. Repo → **Settings → Pages** → Source „Deploy from a branch", Branch `main`, Ordner `/root`.
4. Nach wenigen Minuten unter `https://<user>.github.io/<repo>/` erreichbar.

QR-Codes erst zum Schluss erzeugen und auf die **finale** Adresse zeigen lassen.

## Anpassen
- **Zielseiten austauschen:** `lorem_de.html` / `lorem_nl.html` durch die echten Seiten ersetzen (Dateinamen beibehalten → Links bleiben gültig).
- **Umarmung justieren:** die Überlappung/Größe steckt in `index.html` in `.hero .eagle` / `.hero .lion` (Werte `left` und `height`).
- **Farben/Schrift:** oben in `index.html` unter `:root` bzw. den Google-Fonts (Cormorant Garamond + Jost).
