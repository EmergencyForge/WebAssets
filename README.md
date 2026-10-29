# WebAssets

Statische Dateien von EmergencyForge unter https://web-assets.emergencyforge.de: Logos, Partnerlogos und
Schriften. Bilder unter `images/` bekommen automatisch eine WebP-Fassung in `gen/`.

## Schrift Esse

Esse ist die Hausschrift von EmergencyForge, Esse Mono die Schrift für Code, Zeiten und Tabellen. Beide
bauen auf Geist auf und stehen unter der SIL Open Font License 1.1 (`fonts/esse/OFL.txt`). Quelle und
Bau-Skript liegen in WebPackages unter `packages/esse`.

Einbinden in HTML, zum Beispiel im Tebex-Template:

```html
<link rel="stylesheet" href="https://web-assets.emergencyforge.de/fonts/esse/1.5/esse.css">
```

Oder in CSS:

```css
@import url("https://web-assets.emergencyforge.de/fonts/esse/1.5/esse.css");

body { font-family: "Esse", system-ui, sans-serif; }
code { font-family: "Esse Mono", ui-monospace, monospace; }
```

`fonts/esse/1.5/` ändert sich nie, eine neue Version bekommt einen eigenen Ordner.
`fonts/esse/esse.css` zeigt immer auf die aktuelle Version, für Seiten, die automatisch mitziehen sollen.

Jede Datei enthält alle Stärken von 100 bis 900 (`font-weight` frei wählbar) und die Kursive. Für Uhrzeiten
und Preise `font-variant-numeric: tabular-nums` setzen.
