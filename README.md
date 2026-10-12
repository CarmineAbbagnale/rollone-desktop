# RollOne: repository di aggiornamenti

Repository di distribuzione per RollOne (ora Fumble RPG, compagno D&D 5e e Pathfinder 2e). Sito ufficiale: https://carmineabbagnale.github.io/fumblerpg-site/

- `version.json`: manifest controllato dall'app ad ogni avvio (Windows, macOS, Android) per verificare se è disponibile un aggiornamento dei contenuti.
- `rollone.html`: contenuto dell'app, scaricato automaticamente quando la versione cambia.

Per pubblicare un aggiornamento: sostituire `rollone.html`, calcolare il nuovo sha256, aggiornare `version.json` (campo `version` e `sha256`), fare commit e push su `main`. Tutte le app lo rilevano da sole al successivo avvio.
