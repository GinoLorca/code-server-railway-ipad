# Chess Rating Reveal

A single-file, no-install tool for showing a chess student's rating growth with an animated before/after reveal. Built for testing in the classroom before deciding whether to invest in a full multi-coach version.

## What it does

- Upload a "starting" and a "peak/current" photo for a student
- Enter their name, optional school, an event (Summer Camp, State Championships, Elementary Nationals, ICN Saturday Team Tournament, ICN Saturday Grand Prix, or a custom one), and the two ratings
- Click **Save & reveal growth** for an animated before/after: the rating counts up and an arrow draws in, then replay it anytime
- Every save is kept in a **Roster history** list on that device, automatically grouped under the same student profile by name (so entries from different tournaments/camps stack up over time)

## What's intentionally left out of this test version

- No coach accounts or login — anyone with the file/link can use it
- No server-side photo storage — photos are only used live for the reveal and are **not** saved with history (only name, school, event and ratings persist)
- History lives in the browser's local storage on that one device only — it won't sync across devices or coaches, and clearing browser data clears it

These were cut deliberately to keep this a zero-setup tool for classroom testing. If it proves useful, the natural next step is the fuller version discussed separately: individual coach accounts, real photo storage, and shared history across the whole coaching network.

## How to use it

Open [`2026-09-16-chess-rating-reveal.html`](./2026-09-16-chess-rating-reveal.html) directly in a browser (double-click the file, or drag it into a browser tab). No build step, no server required.

To host it for easier sharing later (e.g. GitHub Pages), copy or rename that file to `index.html`.
