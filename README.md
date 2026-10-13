# Progress traps, claims, evidence, reasoning

A click-through activity for Charlie's New Media 11 persuasive essay unit (session 1).

Open `index.html` in any browser. No build step, no internet needed.

Two parts, chosen from the home screen:

1. **Four words** — the click-through lesson: progress trap, claim, evidence, reasoning.
2. **Real or fake?** — four rounds of two-button items. Local headlines, common myths, misattributed quotes, and what counts as evidence. No score, no timer.

- Back / Next buttons, or left and right arrow keys
- "Read it to me" speaks the current screen using the browser's own voice
- 10 screens: the pattern, progress trap, is-it-a-progress-trap (6), claim or evidence (8), reasoning, which-one-is-the-reasoning (3), where do you stand, the film, recap

## Editing the questions

All the content lives in lists inside the `<script>` block at the bottom of `index.html`:

**Lesson rounds**

- `PT` — is-it-a-progress-trap items (`t` = scenario, `a` = true/false, `img` = image filename without .jpg, `why` = feedback)
- `CE` — claim-or-evidence items
- `RS` — which-one-is-the-reasoning items

**Real or fake rounds**

- `ROUNDS` — one entry per round. Each has a `name`, a `blurb`, the two button `labels`, and its `items`.
- Each item: `q` (what he sees), `who` (optional source line), `a` (which label is correct), `fb` (the verdict), `tell` (how he could have known).

Add or change entries there, nothing else needs touching.

## Sources used in the local round

- CBC, "Metro Vancouver shutting down rogue bike trails on North Shore"
- CBC, "How pandemic bike lanes made some Canadian cities more accessible" (March 2021)
- Globe and Mail, Vancouver bike lanes, quoting UBC researcher Kay Teschke on Seville's 120 km

The made-up headlines in that round are written to sit beside the real ones. Check the real ones before using them if time has passed.

## Images

In `images/`. Photos from Unsplash. Any image that's missing just disappears from the page, so you can swap or delete freely.
