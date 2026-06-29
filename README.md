# Patente A/B — Vero o Falso study console

An offline, single-file study tool for the Italian **Patente A/B** driving theory exam. It turns the official true/false question listing into a trainer with sign images, answer explanations, and a data-driven breakdown of the wording tricks the exam uses.

**Live version:** https://YOUR-USERNAME.github.io/patente/
*(replace with your GitHub Pages URL once it is live)*

---

## What it is

The exam is 30 true/false statements with a pass mark of at most 3 errors. Because the source listing labels every statement as true or false, this tool can do two useful things that a plain question bank cannot:

1. Show you, with exact counts, which Italian words and phrases pull an answer toward **VERO** or **FALSO**.
2. For every sign question, show the actual sign and, when you answer, explain what the sign really means.

Everything is built from the listing itself. Nothing is invented.

## Features

The console is one page with seven tabs:

- **Trainer** — drill statements as Vero or Falso (keys `V` / `F` / `Space`). Sign questions show the sign. When you answer, the result is revealed with a short explanation of why, plus the correct facts from the same question block.
- **Signs** — recognition trainer for the *segnaletica*. Flashcards and a gallery for all 326 signs, grouped by category, each with its true meaning and the trap wordings used against it. Includes the shape-and-colour key for every category.
- **Word signals** — for each tracked word or phrase, the exact share of statements that are true, shown as a bar. Click a word to see its questions.
- **Patterns & traps** — the recurring true patterns, false traps, and the near-twin pairs where one word flips the answer.
- **Sure things** — the deterministic tells: phrases that are 100% one way in the listing, the exact numbers to memorise, and the structural traps.
- **Browse all** — search every statement, filter by topic and by answer. Sign statements show a thumbnail.
- **Cheat sheet** — a one-screen revision pass built around certainties rather than percentages.

## The data

- **7,144** statements (3,568 true / 3,576 false) across **708** blocks and 31 topic areas.
- **326** sign images across 11 categories (danger, prohibition, obligation, priority, indication, temporary, panels, traffic lights, road markings, vehicle lights, dashboard symbols), extracted directly from the source PDF.
- **3,427** statements (the *segnaletica* half) are linked to their sign image.

Source: *Listato ministeriale A/B* (Neca), web version dated 27/02/2025. The answers are the listing's own labels.

## How to use it

- **Online:** open the live URL above.
- **Offline:** download `index.html` and open it in any browser. The data and all sign images are embedded, so it works without internet. The only thing that needs a connection is the web font, which falls back to a system font otherwise.

No build step, no dependencies, no tracking. It is a single static HTML file.

## Hosting it yourself (GitHub Pages)

1. Create a public repository and upload `index.html`.
2. Go to **Settings → Pages**.
3. Set **Source** to **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. The site goes live at `https://YOUR-USERNAME.github.io/REPO-NAME/` within a minute or two.

To update later, replace `index.html` and Pages redeploys automatically.

## Notes and honesty flags

- The percentage signals are statistical tendencies, not laws. Treat them as where to be careful, and the "Sure things" tab as where you can be confident.
- A few sign tells depend on the picture, so they mean "when you see this exact wording the answer was X", not a standalone rule.
- A small number of indication and marking blocks whose figure region came out blank were not cropped, so those few questions show wording only.
- This is a study aid, not official material and not legal advice. Always confirm against the current Codice della Strada.

## Companion files

If you keep them alongside the console:

- `Patente_AB_master.xlsx` — every statement with topic, scenario, answer and keyword tags, plus keyword and scenario analysis sheets.
- `Patente_study_guide.md` — printable guide with the full keyword tables, patterns, scenario index and ranking.
- `Patente_deterministic_patterns.md` — just the certainties: exact numbers, structural traps, and 100% phrase tells.

---

*In bocca al lupo.*
