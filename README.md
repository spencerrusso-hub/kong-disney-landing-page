# Kong × The Walt Disney Company — prospect landing page

Single-file static site. No build step.

- `index.html` — the whole page (CSS + HTML + a few lines of JS for tabs and deep links like `/#parks`)
- `images/kong-mark.png` — Kong logo mark (current lime-on-black brand)

## Editing

Open `index.html` in any editor. Each tab is a `<div class="tab-panel" id="tab-…">` block containing:

1. `.panel-header` — kicker, headline, paragraph, and the `.force-multiplier` proof stat
2. `.cards-grid` — three `.job-card`s (real Disney postings, linked)
3. `.usecase-grid` — four `.usecase-card`s mapping to Kong products
4. `.summary` — Biggest unlock / What it protects / Where to start

Brand tokens live in `:root` at the top of the `<style>` block (Kong lime `#CCFF00`, night `#070807`, Disney blue `#0063E5`).

## Deploying

Import the repo into Vercel (Framework preset: **Other**, no build command, output directory `/`). Every push to `main` redeploys.

## Sources

Role data from public postings on disneycareers.com (September 2026). Kong proof points from konghq.com customer stories, the GigaOm API & Microservices Management Benchmark, Gartner Magic Quadrant for API Management (Oct 2025), and Forrester Wave: API Management Software (Q3 2026). Verify posting wording on the live page before quoting externally.
