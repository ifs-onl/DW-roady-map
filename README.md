# IFS Loops · The agentic journey

A 12-slide customer-facing presentation on the IFS Loops product journey, FY26–27. Single-file HTML deck, no build step, no server required.

## Running it

**Hosted:** enable GitHub Pages on this repo (Settings → Pages → Deploy from branch → `main` / root). The deck is served at the repo's Pages URL.

**Locally:** open `index.html` in any modern browser. It works from `file://` as well as over HTTP.

## Presenter controls

| Key | Action |
| --- | --- |
| `→` `←` `Space` | Next / previous slide |
| `Home` `End` | Jump to first / last |
| `N` | Toggle the speaker-notes panel |
| `Shift` + `N` | Detach notes into a second window (for a side screen) |
| `O` | Overview grid — click to jump, drag to reorder |
| `R` | Reset slide order (in overview) |
| `H` | Hide the current slide, or the hovered slide in overview |
| `Shift` + `H` | Hidden-slides picker |
| `U` | Restore all hidden slides |
| `F` | Fullscreen |
| `?` | Help overlay |

Slide order and hidden slides persist in `localStorage`.

## Interactive content

Two slides carry D3 diagrams driven by hover:

- **Slide 5 — Industrial context graph.** Hover a domain to trace its relationships; hover the core for the summary.
- **Slide 7 — Agentic FSM handover chain.** Hover a worker to highlight its handovers and see what it owns.

Cards on slides 2, 3, 4, 6 and 10 open a detail panel on hover. Roadmap rows and proof tiles respond to hover as well.

## Repository layout

```
index.html          the deck (self-contained markup, CSS and JS)
assets/
  fonts.css         @font-face rules for Inter Tight + JetBrains Mono
  d3.min.js         D3 v7, bundled locally
  IFSLogo_white.png IFS mark
.nojekyll           tells GitHub Pages to serve the site as-is
```

Web font files are fetched from `fonts.gstatic.com` at runtime. Everything else is local, so the deck degrades to system fonts offline rather than breaking.

## Notes on the content

Roadmap timing beyond Q3 FY26 is indicative scope, not a commitment. Roadmap availability is also not the same thing as IFS version support — confirm a customer's release against the IFS version support matrix before scoping.
