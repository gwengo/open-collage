Thanks for adding to the archive. This document covers everything you need to submit assets or fix something in the repository. 

---

## What we accept

Assets from any source, as long as the license is clean:

- **Original work** — you made it, you own it, you're releasing it under CC BY 4.0
- **Freely licensed found material** — CC0, CC BY, or CC BY-SA sources (note the original source in your PR)
- **Public domain material** — anything old enough or explicitly released (note the source)

If you didn't make it, include a link to the original source and its license in your pull request description. If there's any ambiguity about the license, don't submit it.

---

## Technical spec

These requirements are firm. PRs that don't meet them will be sent back, not rejected — just fix and resubmit.

**Format**

- PNG only
- Transparent background (no white, no black, no color fill behind the subject)
- RGB color mode
- No compression artifacts

**Resolution**

- 600dpi minimum for scanned material
- 1500px minimum on the longest edge for photographic or digital sources
- When in doubt, go higher — you can't recover resolution later

**File size**

- Under 20MB per file
- If your asset is larger, export at slightly lower resolution or crop to the essential area

**Naming convention**

```
series-quality-number.png
```

All lowercase. Hyphens, not underscores, not spaces. Examples:

```
river-texture-01.png
studio-edge-03.png
found-type-02.png
archive-photo-01.png
```

If your asset doesn't belong to a series yet, use a short descriptor for the series slot: `scan-`, `photo-`, `found-`, `draw-`.

Numbers are zero-padded to two digits: `01`, `02`, not `1`, `2`.

---

## Folder placement

Put your asset in the folder that matches what it *does*, not what it is technically.

```
curated/      — do not submit here directly; assets move here after review
open/
  texture/    — surface, grain, noise, material
  edge/       — borders, cuts, torn edges, dividing lines
  mark/       — discrete gestures, stamps, single strokes
  ground/     — large areas, fields, washes, backgrounds
  figure/     — isolated shapes with clear silhouette
  void/       — negative space, open areas, absence
  pattern/    — repeating elements, grids, tessellation
  type/       — letterforms, hand-lettered, printed text fragments
  photo/      — photographic fragments, halftones, reproductions
```

All submissions go into `open/` first. Don't submit directly to `curated/` — assets move there after review.

If you're genuinely unsure which folder fits, pick the closest one and mention it in your PR. We can move it.

---

## How to submit

1. Fork the repository
2. Add your asset(s) to the correct folder under `open/`
3. Name files to convention
4. Open a pull request against `main`

Your PR description should include:

- What the asset is and how it was made or where it came from
- License confirmation: *"This is my original work and I release it under CC BY 4.0"* or a link to the source license
- Which folder you chose and why, if it's not obvious


---

## Pull request checklist

Before submitting, check:

- [ ]  PNG format with transparent background
- [ ]  600dpi / 1500px minimum resolution
- [ ]  Under 20MB per file
- [ ]  Named to convention (`series-quality-number.png`)
- [ ]  Placed in the correct folder under `open/`
- [ ]  PR description includes source and license confirmation

---

## Review

PRs are reviewed on a rolling basis. If something doesn't meet spec, you'll get a note explaining what to fix. If the folder placement seems off, we'll suggest a move. We won't reject assets on aesthetic grounds.

Once merged, assets sit in `open/`. Over time, well-used and high-quality assets move into `curated/` — but that's not something contributors need to do or track.

---

## Other contributions

Found a bug, broken link, or something wrong in the documentation? Open an issue or submit a PR directly — small fixes don't need much explanation.

Want to contribute a tool (p5.js script, processing workflow, etc.)? Add it to `/tools` with its own short README and open a PR. Same license applies.

Questions? Open an issue and ask.
