# School crest files

Drop each official school logo here as an SVG, then add a matching entry to
`SCHOOL_LOGOS` in `chess-league/index.html` (right after `SCHOOL_COLORS`):

```js
const SCHOOL_LOGOS = {
  "PS 11": "logos/ps-11.svg",
  "Nest+M": "logos/nest-m.svg",
  ...
};
```

The key must be the exact school name used in `LEAGUE_DATA`. The file itself
can be any aspect ratio — wide, tall, or square — the app displays it inside
a fixed 24x24 box with `object-fit: contain` (see `.team-logo` in the
`<style>` block), so mismatched proportions are automatically centered and
scaled without distortion or cropping.

A school with no entry here just falls back to its `SCHOOL_COLORS` swatch,
or a blank space if it has neither.

## Pending: schools with a matched logo, not yet added

These 35 schools were matched against their official crest (uploaded to
Google Drive) but the actual SVG files haven't been pulled in yet. Filename
slugs to use once each file is added:

| School | File |
|---|---|
| A-S | logos/a-s.svg |
| BASIS-B | logos/basis-b.svg |
| Brooklyn Prospect IES | logos/brooklyn-prospect-ies.svg |
| BSI | logos/bsi.svg |
| Nest+M | logos/nest-m.svg |
| PS 3 | logos/ps-3.svg |
| PS 10 | logos/ps-10.svg |
| PS 11 | logos/ps-11.svg |
| PS 111 | logos/ps-111.svg |
| PS 116 | logos/ps-116.svg |
| PS 118 | logos/ps-118.svg |
| PS 124 | logos/ps-124.svg |
| PS 130 | logos/ps-130.svg |
| PS 130M | logos/ps-130m.svg |
| PS 166 | logos/ps-166.svg |
| PS 184M | logos/ps-184m.svg |
| PS 198 | logos/ps-198.svg |
| PS 20 | logos/ps-20.svg |
| PS 230 | logos/ps-230.svg |
| PS 281 | logos/ps-281.svg |
| PS 282 | logos/ps-282.svg |
| PS 290 | logos/ps-290.svg |
| PS 31 | logos/ps-31.svg |
| PS 32 | logos/ps-32.svg |
| PS 33 | logos/ps-33.svg |
| PS 333 | logos/ps-333.svg |
| PS 34 | logos/ps-34.svg |
| PS 340 | logos/ps-340.svg |
| PS 39 | logos/ps-39.svg |
| PS 40 | logos/ps-40.svg |
| PS 527 | logos/ps-527.svg |
| PS 59 | logos/ps-59.svg |
| PS 77 | logos/ps-77.svg |
| PS 889 | logos/ps-889.svg |
| Town School | logos/town-school.svg |

Source: Google Drive `My Drive/Chess/ICN/ICN League/ICN School Logo's`.
Blocked on Drive access for this session — pull these in once reconnected.
