# Sabbatjahr

Statisches Web-Projekt (HTML/JS/Service Worker), das die Arbeitstage bis zum Sabbatjahr-Start zählt und einen Kalender rendert.

## Push-Workaround

`git push origin main` schlägt in dieser Umgebung mit **HTTP 403** fehl (Proxy blockiert). Stattdessen:

- **Direkt auf main schreiben:** `mcp__github__push_files` (GitHub-API, am Proxy vorbei).
- **Über PR:** `mcp__github__create_pull_request`, dann im UI mergen.

Vorher kurz mit dem Nutzer klären, welcher Weg gewünscht ist.
