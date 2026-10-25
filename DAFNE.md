---
format: 0
banks:
  - name: spanish-reading
    bank: ./reading-log
    graduate: false
    patterns:
      - "reading-log/context\\.md"
---

# Spanish Grove

Rioplatense Spanish (Argentine/River Plate dialect) knowledge enclave.
Anki card specification and overall progression.
Literature search and analysis.

## Files in this area

| Path | What |
|---|---|
| `./rioplatense-anki.md` | Main deck context: card types, generation rules, tagging taxonomy. Compiled via DAFNE before card generation. |
| `./focus_area.md` | Rioplatense dialect criteria (voseo, Argentine vocabulary). Injected into card generation and used as the sole extraction context for youtube-extract. |
| `./deck_quality_bootstrapping/` | deck quality & efficiency analysis at a certain snapshot |
| `./reading-log/context.md` | Reading-log area — mem-bank for reading session history. Curating literature, discussing about reading journey |
| `./parents/` | Inherited base nodes (`language` → `deck`), spliced into the deck spec via `#include`. Method and pedagogy research live here — see `parents/language/DAFNE.md` |
| `./files/` | Media files (PDFs, etc.) referenced by cards or resources. |
| `./backups/` | Deck backup archives (.apkg). |

## Workflows

| When | Do |
|---|---|
| A transcript of my spoken Spanish needs turning into cards | Follow `parents/language/transcript-triage.md`. It reads `parents/language/intake-channels.md`, `./focus_area.md` and the gap ledger in this grove's **private layer** (the orientation line names the path), proposes a numbered shortlist, and hands the accepted ones to `/pipe:add-cards-to-grove` in card format. Never feed a raw transcript to that pipeline directly — and never copy transcript or ledger content into a tracked file. |
| I hand over curated phrases or sentences from a book | Straight to `/pipe:add-cards-to-grove` — that is the input contract it already has. |
