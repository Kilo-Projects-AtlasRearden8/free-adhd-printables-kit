# STATUS — Free ADHD Printables Pack

## What was built

A fillable, printable freebies pack for low-energy and ADHD days, made by Asdale Dynamics, LLC.

Files:
- `index.html` — pack landing page linking to all three printables
- `css/style.css` — shared screen + print CSS (kind, small-steps design; print hides buttons/headers)
- `printables/task-cards.html` — one tiny step per card, with done checkbox and printable card stack
- `printables/routine-template.html` — morning, evening, and reset (low-energy) routines
- `printables/energy-tracker.html` — 7-day energy log (1–5) plus "what helped / what drained me"
- `markdown/task-cards.md`, `markdown/routine-template.md`, `markdown/energy-tracker.md` — Markdown sources
- `README.md` — overview, how to use, credit to Asdale Dynamics, LLC
- `LICENSE` — MIT License, copyright line exactly `Copyright (c) 2026 Asdale Dynamics, LLC`

No account needed. No tracking. No secrets, API keys, or personal data. No `.github/workflows`.

## How to run

Open any HTML file directly in a browser:

```
index.html
printables/task-cards.html
printables/routine-template.html
printables/energy-tracker.html
```

Type into fields on screen, then print (Ctrl+P / Cmd+P) or save as PDF. Print styles hide screen-only buttons and headers automatically. Markdown files are plain-text sources; no build step required.

## Verification results

- All 4 HTML files parse as well-formed (Python `html.parser` check): **OK** for index.html, task-cards.html, routine-template.html, energy-tracker.html
- `LICENSE` copyright line is exactly `Copyright (c) 2026 Asdale Dynamics, LLC`: **OK**
- README credits Asdale Dynamics, LLC: **OK**
- No `.github/workflows` directory: **OK**
- Secrets scan (api key / secret / password / sk- / token): no real secrets; only benign matches (file paths, CSS comment, readme links): **OK**
- No build step; pages are static HTML/CSS/Markdown.

## Known gaps

- No automated test suite (static site; validation done via parser check above)
- Print appearance not rendered to PDF visually; relies on `@media print` CSS (verified present, not rendered)
- No dark-mode toggle or user accounts (by design: no account needed, local-first)
- Markdown sources are not auto-generated from HTML; kept in sync manually
