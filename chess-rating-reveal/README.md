# Chess Rating Reveal

A single-file, no-install tool for showing a chess student's rating growth with an animated before/after reveal. Built for testing in the classroom before deciding whether to invest in a full multi-coach version.

## What it does

- Upload a "starting" and a "peak/current" photo for a student — tap to browse, or drag a photo straight in from the desktop
- Enter their name, optional school (with an optional school logo), an event (Summer Camp, State Championships, Elementary Nationals, ICN Saturday Team Tournament, ICN Saturday Grand Prix, or a custom one), and the two ratings
- Pick a card background color (a few presets or a custom color)
- Click **Reveal growth** for the animated payoff: the "after" photo blooms from desaturated into full color exactly as the rating counts up, an arrow draws in, and a gold ring pulses at the finish. Replay it anytime.
- **Save picture** exports the reveal card as a PNG. **Save video** records a short clip of the animation (MP4 where the browser supports it, since that's what Instagram/TikTok/iOS sharing expect; it falls back to WebM only on browsers that can't record MP4, and says so).

## What's intentionally left out of this version

- No coach accounts or login — anyone with the file/link can use it
- No history — each reveal is a one-off; nothing about the student or their ratings is saved anywhere. Use **Save picture** / **Save video** to keep a record of a given reveal.
- No server-side storage of any kind — the only things remembered locally in the browser are a school's logo (so you don't have to re-upload it for the next student from that school) and your last-picked card background color.

These were cut deliberately to keep this a zero-setup tool for classroom testing. If it proves useful, the natural next step is the fuller version discussed separately: individual coach accounts, real photo storage, and shared history across the whole coaching network.

## How to use it

Open [`2026-09-16-chess-rating-reveal.html`](./2026-09-16-chess-rating-reveal.html) directly in a browser (double-click the file, or drag it into a browser tab). No build step, no server required.

To host it for easier sharing later (e.g. GitHub Pages), copy or rename that file to `index.html`.

Video export relies on browser APIs (`MediaRecorder` + canvas capture) — this works in current Safari (including iPadOS) and Chromium browsers. Picture export works everywhere.
