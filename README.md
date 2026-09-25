# tres_site

Marketing site for **Treslabs** — an AI-native customer experience platform for voice agents.

## Contents

| File | What it is |
|------|------------|
| `index.html` | **V2 — Refined.** The current design. Light and dark themes, full interaction system. |
| `treslabs-v1.html` | **V1 — Current.** The earlier direction, kept for comparison. |

Both are single self-contained files — no build step, no dependencies. Open either
directly in a browser, or serve the folder with any static server.

## Prototype controls

A discreet control panel sits at the **bottom-left** of each page. It is a design
tool, not part of the product navigation:

- **Version** — switch between V1 and V2
- **Theme** — Light / Dark / System (V2 only; the choice persists in `localStorage`)

## Design system, in brief

- **Primitive:** the *trace* — a conversation drawn as a line in time. Speech is
  density on the line, events are marks on it, many traces stacked are the system.
  Every graphic on the page is that one component with different data.
- **Colour:** graphite, warm bone, and a single signal citron. Citron is never text
  or a hairline on a light surface; there it appears only as a filled marker or on a
  deliberate graphite operational surface.
- **Type:** Instrument Sans throughout, with IBM Plex Mono reserved for genuine
  machine data — timestamps, call IDs, counts.
- **Motion:** semantic only. Nothing animates to decorate; traces draw, data updates,
  and the lifecycle changes state. `prefers-reduced-motion` is respected.

## ⚠️ All data is placeholder

Every metric, call transcript, customer category and system event on these pages is
**invented for design purposes**. Nothing here reflects real product performance,
real customers, or real compliance status. Replace before any public use.

## Local preview

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000
