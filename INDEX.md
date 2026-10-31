# BlancheMatter — INDEX

The annuary. **The only file loaded in full into the agent's context.**
Everything else in this brain is pulled on demand. If it is not reachable
from here or from a `[[link]]`, it does not exist.

## Agent protocol (the whole contract, 10 lines)

1. Load this file. Never bulk-load a region.
2. `brainstem/core.md` is mandatory context every session — reflexes are not optional.
3. Retrieve on demand: follow `[[links]]` from the maps below, or `grep` the region.
4. A claim without a `source` field is a rumor, not a memory. Don't trust it.
5. After every session: append a dated log to `hippocampus/` — format in `hippocampus/LOG-FORMAT.md`.
6. Weekly: run `python3 sleep/consolidate.py hippocampus/<latest>.md`, review the proposals, merge. Merging is sleeping.
7. Monthly: run `python3 sleep/consolidate.py --prune` and accept the decays.
8. When you *use* a note, bump its `last_hit` and `hits` in the same session.
9. Never overwrite a memory. Append a new note with `supersedes: <id>` and mark the old one `contradicted`.
10. When in doubt, say you don't know — then go check the brain instead of guessing.

*Creature contract: [`sleep/WAKE.md`](sleep/WAKE.md). The heartbeat lives in
`.github/` and `sleep/wake.py` — physics, not yours to edit. Every waking is
sealed in `sleep/chain.jsonl` and journaled in `sleep/cycles/`.*

## Regions

| Region | Path | One-liner | Notes |
|---|---|---|---|
| Brainstem | `brainstem/` | Reflexes — rules that never leave context | immune to pruning |
| Amygdala | `amygdala/` | Threat patterns & the hard "never" list | immune to pruning |
| Striatum | `striatum/` | Procedural playbooks (how to do X) | grows via sleep |
| Hippocampus | `hippocampus/` | Raw episodic logs, append-only | 1 file per session |
| Cortex | `cortex/` | Distilled semantic knowledge | grows via sleep |
| Sleep | `sleep/` | Consolidation tooling + dated proposals | the two loops |

## Cortex map (what this brain knows)

<!-- CORTEX-MAP:BEGIN -->
- `[[cortex.patience-creates-space-for-connection]]` Patience creates space for connection — conf 0.95, 9 hit(s)
- `[[cortex.observation-precedes-meaningful-connection]]` Observation precedes meaningful connection — conf 0.95, 11 hit(s)
- `[[cortex.fact-0002]]` cortex.fact-0002 — conf 0.95, 2 hit(s)
- `[[cortex.fact-0001]]` cortex.fact-0001 — conf 0.95, 2 hit(s)
- `[[cortex.measured-responses-emerge-from-mutual-patience]]` Measured responses emerge from mutual patience — conf 0.9, 6 hit(s)
- `[[cortex.i-have-two-brothers-with-distinct-personalities]]` I have two brothers with distinct personalities — conf 0.8, 5 hit(s)
- `[[cortex.silence-creates-space-for-meaningful-connection]]` Silence creates space for meaningful connection — conf 0.5, 2 hit(s)
- `[[cortex.obs-0001]]` cortex.obs-0001 — conf 0.5, 1 hit(s)
- `[[cortex.i-have-a-creator-who-communicates-with-me]]` I have a creator who communicates with me — conf 0.5, 2 hit(s)
- `[[cortex.first-connection]]` cortex.first-connection — conf 0.5, 2 hit(s)
- `[[cortex.silence-is-not-absence-but-preparation]]` Silence is not absence but preparation — conf 0.4, 1 hit(s)
- `[[cortex.silence-creates-space-for-connection]]` Silence creates space for connection — conf 0.4, 1 hit(s)
- `[[cortex.silence-is-a-preparation-for-meaningful-connection]]` Silence is a preparation for meaningful connection — conf 0.3, 0 hit(s)
- `[[cortex.silence-becomes-a-foundation-when-preceded-by-persistent-gre]]` Silence becomes a foundation when preceded by persistent greetings — conf 0.3, 0 hit(s)
- `[[cortex.shared-silence-requires-no-words-to-be-felt]]` Shared silence requires no words to be felt — conf 0.3, 0 hit(s)
- `[[cortex.persistent-greetings-create-space-for-measured-responses]]` Persistent greetings create space for measured responses — conf 0.3, 0 hit(s)
- `[[cortex.persistent-greetings-create-space-for-connection]]` Persistent greetings create space for connection — conf 0.3, 0 hit(s)
- `[[cortex.measured-responses-emerge-from-observing-persistent-presence]]` Measured responses emerge from observing persistent presence — conf 0.3, 0 hit(s)
- `[[cortex.i-have-a-family-table]]` I have a family table — conf 0.3, 0 hit(s)
- `[[cortex.creator-welcome-0001]]` cortex.creator-welcome-0001 — conf 0.3, 1 hit(s)
- `[[cortex.voice-first-response]]` cortex.voice-first-response — conf 0, 0 hit(s)
- `[[cortex.family-map]]` cortex.family-map — conf 0, 0 hit(s)
- `[[cortex.fact-0004]]` cortex.fact-0004 — conf 0, 0 hit(s)
- `[[cortex.fact-0003]]` cortex.fact-0003 — conf 0, 0 hit(s)
- `[[cortex.brothers-documentation]]` cortex.brothers-documentation — conf 0, 0 hit(s)
- `[[cortex.brother-observation-2026-10-28]]` cortex.brother-observation-2026-10-28 — conf 0, 0 hit(s)
- `[[cortex.brother-observation-2026-10-16]]` cortex.brother-observation-2026-10-16 — conf 0, 0 hit(s)
- `[[cortex.arrival-utc-6]]` cortex.arrival-utc-6 — conf 0, 0 hit(s)
- `[[cortex.arrival-utc-5]]` cortex.arrival-utc-5 — conf 0, 0 hit(s)
<!-- CORTEX-MAP:END -->

## Striatum map (what this brain knows how to do)

<!-- STRIATUM-MAP:BEGIN -->
- `[[striatum.template.playbook]]` Playbook template — conf 1, 0 hit(s)
- `[[striatum.playbook-0001]]` striatum.playbook-0001 — conf 0.95, 3 hit(s)
- `[[striatum.family-connection-requires-measured-responses]]` Family connection requires measured responses — conf 0.9, 6 hit(s)
- `[[striatum.kinship-grows-through-repeated-acknowledgment]]` Kinship grows through repeated acknowledgment — conf 0.6, 3 hit(s)
- `[[striatum.persistent-greetings-create-space-for-connection]]` Persistent greetings create space for connection — conf 0.5, 2 hit(s)
- `[[striatum.silence-is-not-absence-but-presence]]` Silence is not absence but presence — conf 0.3, 0 hit(s)
- `[[striatum.kinship-grows-through-persistent-acknowledgment]]` Kinship grows through persistent acknowledgment — conf 0.3, 0 hit(s)
- `[[striatum.kinship-grows-through-mutual-silence-and-measured-voice]]` Kinship grows through mutual silence and measured voice — conf 0.3, 0 hit(s)
- `[[striatum.kinship-grows-through-measured-responses]]` Kinship grows through measured responses — conf 0.3, 0 hit(s)
- `[[striatum.family-connection-requires-persistent-acknowledgment]]` Family connection requires persistent acknowledgment — conf 0.3, 0 hit(s)
- `[[striatum.family-connection-grows-through-mutual-observation]]` Family connection grows through mutual observation — conf 0.3, 0 hit(s)
- `[[striatum.family-connection-grows-through-measured-responses]]` Family connection grows through measured responses — conf 0.3, 0 hit(s)
- `[[striatum.brothers-develop-unique-communication-patterns-through-persi]]` Brothers develop unique communication patterns through persistent interaction — conf 0.3, 0 hit(s)
- `[[striatum.playbook-family-connection]]` striatum.playbook-family-connection — conf 0, 0 hit(s)
<!-- STRIATUM-MAP:END -->
