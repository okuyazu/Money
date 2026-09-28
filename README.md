# Money 💵

A personal, **local-first** finance app — accounts, spending, budget, and
reports over a small Markdown vault. Runs as an installable app on your phone or
in any browser, works fully offline, and optionally syncs to this GitHub repo.

- 📊 **Overview / Transactions / Budget / Reports** tabs
- 🧾 **Add transactions** by hand, **import a CSV** statement, or **import from a
  bank-app screenshot** (text is read on-device; the image is never uploaded)
- 💾 **Local-first** — everything is stored on your device; no login needed
- 🔄 **Optional GitHub sync** — paste a fine-grained token to keep a Markdown
  copy and sync across devices
- 📦 **Zero build** — plain HTML/CSS/JS

## Data
Lives in [`money/`](money/) as Markdown:
- `accounts.md` — your accounts
- `budget.md` — categories, monthly limits, and `## Rules` keywords for
  auto-categorising
- `index.json` — the list of month ledgers
- `YYYY-MM.md` — one ledger table per month

## Publishing (GitHub Pages)
**Settings → Pages → Build and deployment → Source: Deploy from a branch →
Branch: `main` / root.** The app is then live at
`https://<username>.github.io/money/`.

## Run locally
```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

---

_Split out from the [My Benchmarks](https://github.com/okuyazu/routine) project
so finance lives on its own._
