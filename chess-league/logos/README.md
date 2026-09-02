# School crest files

Each official school logo lives here as an SVG (optimized with svgo), and is
wired up in `SCHOOL_LOGOS` in `chess-league/index.html` (right after
`SCHOOL_COLORS`):

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

Source: Google Drive `My Drive/Chess/ICN/ICN League/ICN School Logo's`. The
following schools had a logo uploaded there with no matching school in the
app's data, so their crest was not added: Poly Prep, St. Hilda's & St.
Hugh's, PS 56, PS 343, PS 217, PS 133, Harlem Academy, Brooklyn Prospect SY,
Brooklyn Prospect DT.
