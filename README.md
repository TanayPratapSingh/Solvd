# Solvd

Concept landing page for a workspace built around collective problem solving.

**Live:** https://tanaypratapsingh.github.io/Solvd/

## The idea

Problems in, validated solutions out. One place to post a problem, fund a bounty against it, review
every solution built for it, argue the trade offs in the open, and track which solution actually
gets adopted.

The framing the page leans on: not a forum, but a system for getting things solved. Discussion
threads produce opinions. This produces an adoption record.

## Four steps

The page walks a problem through its lifecycle:

1. **Post** the problem
2. **Build** solutions against it
3. **Discuss** the trade offs between them
4. **Adopt** the one that wins

## Features presented

| Feature | What it covers |
| --- | --- |
| Funded bounties | Money attached to a problem so solving it is worth someone's time |
| Verified outcomes | A record of what was actually adopted, not just proposed |
| Solver reputation | Track record built from adopted solutions |
| AI synthesis | Condensing many competing solutions into a comparable view |
| Build workspace | Where solutions get made, not just described |
| Private team spaces | Internal problems that should not be public |

The thesis stated on the page: the moat is the data, not the chatter. The value accrues in the
record of which solutions were adopted and why, not in discussion volume.

## Implementation

A single self contained `index.html`, roughly 480 lines, no build step and no dependencies beyond
web fonts.

- Editorial visual style with a light and dark theme, switched through a `data-theme` attribute on
  `html` and driven entirely by CSS custom properties
- Typography from Google Fonts: Newsreader for display serif, Inter Tight for interface text, and
  Spline Sans Mono for labels
- Sticky navigation with a blurred translucent background using `backdrop-filter` and `color-mix`
- Responsive down to mobile, with the nav collapsing to a burger under 760px

## Running it

No build required. Open `index.html` in a browser, or serve the directory:

```bash
python3 -m http.server 8000
```

## Status

This is a concept and positioning page. There is no application behind it yet.
