<!-- Dieser PR läuft durch die "Vault Checks"-CI (Link-Integrität + Schreibbereich). -->

## Art des Beitrags
- [ ] **Draft** — nur Änderungen in meinem eigenen `drafts/<name>/`-Silo
- [ ] **Promotion** — Entwurf wird in den Kanon (00–12) gehoben (nur Maintainer)
- [ ] **Infrastruktur** — Tools / CI / Regeldateien (nur Maintainer)

## Worum geht es?
<!-- 1–3 Sätze. Bei einer Paper-/Konzept-Notiz: welcher Stream / welche Map? -->

## Checkliste
- [ ] Ich habe **nur in meinem Silo** geschrieben (falls Draft) — CI-Schreibbereich grün.
- [ ] Keine toten `[[Wikilinks]]` — `python tools/check_links.py` läuft grün.
- [ ] Bei Promotion: **rückwärts verlinkt** (mind. ein Research Stream *oder* eine Literature Map zeigt auf die Notiz).
- [ ] Bei Promotion: Dedup geprüft (`python tools/check_dedup.py <datei>`) — kein Duplikat zu bestehender Kanon-Notiz.
- [ ] `.obsidian/` nicht unbeabsichtigt mit-committet.
