# Sabbatjahr Countdown PWA

Mini-App, die als vollwertige App auf dem Handy installiert werden kann.

## Inhalt
- `index.html` – die App selbst (kein Build nötig, reines HTML/CSS/JS)
- `manifest.json` – PWA-Manifest
- `sw.js` – Service Worker (für Offline-Nutzung)
- `icon-192.png`, `icon-512.png` – App-Icons

## Auf GitHub Pages veröffentlichen

1. Neues Repo auf GitHub erstellen, z. B. `sabbatjahr`.
2. Alle Dateien aus diesem Ordner ins Repo hochladen (per Web-Upload oder `git push`).
3. Im Repo: **Settings → Pages → Branch: `main` / `(root)` → Save**.
4. Nach 1–2 Minuten ist die App erreichbar unter:
   `https://<dein-github-name>.github.io/sabbatjahr/`

## Auf dem Handy installieren

**iPhone (Safari):**
- URL öffnen → Teilen-Button → "Zum Home-Bildschirm"

**Android (Chrome):**
- URL öffnen → Menü (⋮) → "App installieren" oder "Zum Startbildschirm hinzufügen"

Nach der Installation öffnet sich die App **vollbild ohne Browser-Leiste**.

## Offline
Der Service Worker cached alles beim ersten Aufruf – die App läuft danach auch offline.

## Anpassen
Alle Daten stehen oben in `index.html` im `<script>`-Block:
- `SABBAT_START` – Startdatum
- `HOLIDAYS` – gesetzliche Feiertage
- `EXTRA_FREE` – zusätzliche freie Tage
