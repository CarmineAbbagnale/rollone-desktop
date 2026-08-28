# RollOne — aggiornamenti

Repository di distribuzione per RollOne (compagno D&D 5e).

- `version.json`: manifest controllato dall'app ad ogni avvio (Windows, macOS, Android) per verificare se è disponibile un aggiornamento dei contenuti.
- `rollone.html`: contenuto dell'app, scaricato automaticamente quando la versione cambia.

Per pubblicare un aggiornamento: sostituire `rollone.html`, calcolare il nuovo sha256, aggiornare `version.json` (campo `version` e `sha256`), fare commit e push su `main`. Tutte le app lo rilevano da sole al successivo avvio.
