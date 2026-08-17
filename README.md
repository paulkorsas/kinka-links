# Kinka Coloring Books – QR-Code Redirects

Diese Seiten leiten von einem festen QR-Code-Ziel auf die jeweilige Amazon-Produktseite weiter.
Der QR-Code selbst muss nie neu gedruckt werden – nur die ASIN in der jeweiligen `index.html` wird bei Bedarf aktualisiert.

## Setup (einmalig)

1. Dieses Repo zu GitHub hochladen (öffentliches Repo, z.B. `kinka-links`)
2. In den Repo-Einstellungen unter "Pages" → Branch `main`, Ordner `/ (root)` aktivieren
3. Die Seiten sind dann erreichbar unter:
   `https://DEIN-GITHUB-NAME.github.io/kinka-links/ORDNERNAME/`

## Mapping-Übersicht

| Ordner | Buch | ASIN | Status |
|---|---|---|---|
| `/nostalgie/` | Erinnerungen von früher | **PLATZHALTER-ASIN** | ⏳ ASIN nach Launch eintragen |
| `/vogel/` | Vögel im Garten | B0H498GBCB | ✅ live |
| `/schmetterlinge/` | Schmetterlinge im Garten | B0H5TH2MGD | ✅ live |
| `/hunde/` | Treue Hunde | **PLATZHALTER-ASIN** | ⏳ ASIN nach Launch eintragen |
| `/tiere/` | Große Tiermotive | B0GCJSGPHV | ✅ live |
| `/blumen/` | Blumen & Gartenmotive | B0GQCPHZ2D | ✅ live |
| `/blumen-natur/` | Natur & Landschaftsmotive | B0GZYGXSC8 | ✅ live |
| `/alltag/` | Alltagsmotive | B0GJPLNTCQ | ✅ live |

## ASIN aktualisieren (bei Nostalgie und Hunde)

1. Die entsprechende `index.html` öffnen (z.B. `nostalgie/index.html`)
2. `PLATZHALTER-ASIN` an **beiden** Stellen durch die echte ASIN ersetzen
3. Änderung committen/hochladen – fertig, der QR-Code funktioniert sofort

## QR-Codes generieren

Für jedes Buch den QR-Code auf die jeweilige GitHub-Pages-URL zeigen lassen, z.B.:

```
https://DEIN-GITHUB-NAME.github.io/kinka-links/nostalgie/
https://DEIN-GITHUB-NAME.github.io/kinka-links/hunde/
```

Generator: qr-code-generator.com oder qrcode-monkey.com
- Statischer QR-Code (nicht dynamisch)
- Fehlerkorrektur: Mittel oder Hoch
- Export als SVG oder hochauflösendes PNG

Diese QR-Codes können **sofort** erstellt werden, auch bevor die ASIN feststeht – die URL selbst ändert sich nie, nur das Ziel dahinter.
