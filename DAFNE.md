---
format: 0
requires: []
banks:
  - name: spanish-reading
    bank: ./reading-log
    graduate: false
    patterns:
      - "reading-log/context\\.md"
---

# spanish — Rioplatense Spanish grove

A **grove**: a DAFNE node carrying memory (the banks above). The
grove-ness is inferred structurally from the bank declaration — there is
no `type:` field. One parent: `parents/language`.

Rioplatense Spanish (Argentine/River Plate dialect) knowledge enclave.
Anki card specification and overall progression. Literature search and
analysis.

| File | What |
|---|---|
| `./rioplatense-anki.md` | Main deck context — compiled via DAFNE before card generation |
| `./focus_area.md` | Rioplatense dialect criteria (voseo, Argentine vocabulary) |
| `./resources.md` | Source material and reference links |
| `./reading-log/` | mem-bank: reading session history |
| `./deck_quality_bootstrapping/` | Deck quality & efficiency analysis snapshots |
| `./files/` | Source PDFs and reference material |
| `./backups/` | Anki deck backups (`.apkg`, gitignored — restore from AnkiWeb if lost) |

This `banks:` config is a placeholder scaffold — the live subscription source of
truth remains `groves/mem-bank-subscriptions.json` in the monorepo until Phase 3
of the DAFNE execution plan wires mem-bank to read it from here.
