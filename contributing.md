# CONTRIBUTING.md

Thanks for adding to the archive. This document covers everything you need to submit assets or fix something in the repository.

The bar for contributing is technical, not aesthetic. If your asset meets the spec below, it goes in. What it looks like, what process made it, how abstract or representational it is — that's up to you.

---

## What we accept

Assets from any source, as long as the license is clean:

- **Original work** — you made it, you own it, you're releasing it under CC BY 4.0
- **Freely licensed found material** — CC0, CC BY, or CC BY-SA sources (note the original source in your PR)
- **Public domain material** — anything old enough or explicitly released (note the source)

Good sources to draw from: Rijksmuseum, Biodiversity Heritage Library, NYPL Digital Collections, Wellcome Collection, Internet Archive Book Images, Smithsonian Open Access, Europeana (check license per item).

If you didn't make it, include a link to the original source and its license in your pull request. If there's any ambiguity about the license, don't submit it.

---

## Technical spec

These requirements are firm. PRs that don't meet them will be sent back, not rejected — fix and resubmit.

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
- If larger, export at slightly lower resolution or crop to the essential area

**Naming convention**
```
style-subject-number.png
```
All lowercase. Hyphens, not underscores, not spaces. Numbers zero-padded to two digits. Examples:
```
engraving-vehicle-01.png
natural-history-primate-03.png
photograph-portrait-02.png
medieval-monster-01.png
watercolor-botanical-04.png
vernacular-stamp-01.png
```

---

## Folder placement

Put your asset in the folder that matches its style and source type. All submissions go into `open/` first — do not submit directly to `curated/`.

```
open/
  engraving/        — woodcut, etching, lithograph, pen illustration, crosshatch
  natural-history/  — scientific specimen plates, botanical, anatomy, geology
  photograph/       — halftone, photographic reproduction, press photo, portrait
  watercolor/       — painted illustration, wash, hand-colored plates
  medieval/         — manuscript, illuminated, devotional, bestiary, early woodcut
  vernacular/       — ephemera, stamps, labels, packaging, trade cards

curated/            — do not submit here; assets move here after review
  (same subfolders)
```

### Folder definitions

**`engraving/`**
Line-based illustration made for reproduction. The image is built from marks, not tone — woodcut, etching, crosshatch pen drawing. Black and white or limited color, typically 16th–19th century printed matter: books, newspapers, encyclopedias, broadsheets.
*In:* Victorian encyclopedia plates, Doré illustrations, old map cartouches, botanical diagrams, illustrated vehicles and figures.
*Out:* anything painted, anything photographic, anything where line is just an outline rather than the whole image.

**`natural-history/`**
Scientific illustration of specimens — animals, plants, minerals, anatomy, geology, insects. Made to document. Highly detailed, often hand-colored or painted. Subject presented neutrally, as a thing to be examined.
*In:* Biodiversity Heritage Library plates, Wellcome Collection anatomy, geological specimen illustrations, bird and botanical plates.
*Out:* decorative nature illustration where mood matters more than the specimen (that's `watercolor/`); engravings of animals in narrative scenes (that's `engraving/`).

**`photograph/`**
Photographic source material. The image originated as a photograph, even if reproduced through printing and showing halftone grain. Black and white or early color, roughly 1850s–1970s.
*In:* press photography, portrait studio images, newspaper halftones, photobooth images, early documentary photography.
*Out:* contemporary clean stock photography; scanned paintings or illustrations that happen to be photographed.

**`watercolor/`**
Painted illustration where the image is built from wash, tone, and pigment. The difference from `natural-history/` is intent — these images are made to be beautiful or expressive, not purely documentary.
*In:* hand-colored plates where the color does emotional work, children's book illustration, painted maps, decorative botanical art, travel illustration.
*Out:* scientific specimen plates where painting is just accurate description (that's `natural-history/`); anything line-dominant (that's `engraving/`).

**`medieval/`**
Pre-1600 manuscript and early printed imagery. Illuminated manuscripts, marginalia, devotional illustration, bestiaries, alchemical diagrams. Pre-perspectival visual logic — flat figures, symbolic space, bold outline, unmodulated color.
*In:* Book of Hours illustration, alchemical manuscript diagrams, early printed herbals, medieval maps, marginalia creatures.
*Out:* Renaissance painting (too perspectival); Victorian medievalist illustration that imitates the style (that goes in `engraving/` or `watercolor/`).

**`vernacular/`**
Printed ephemera made for everyday use — functional, commercial, made to be discarded. Usually involves type and image together.
*In:* vintage postage stamps, apothecary labels, circus posters, seed packet illustration, matchbook covers, Victorian trade cards.
*Out:* fine art prints made to hang on walls; editorial newspaper illustration (that's `engraving/`).

**Hard edge cases:**
- `natural-history/` vs `watercolor/` — ask: is the painting documentary or expressive?
- `engraving/` vs `vernacular/` — ask: was this made for a book/newspaper, or for a commercial/functional printed object?

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

- [ ] PNG format with transparent background
- [ ] 600dpi minimum (scanned) or 1500px minimum on longest edge (photo/digital)
- [ ] Under 20MB per file
- [ ] Named `style-subject-number.png`
- [ ] Placed in the correct folder under `open/`
- [ ] PR description includes source and license confirmation

---

## Review

PRs are reviewed on a rolling basis. If something doesn't meet spec, you'll get a note explaining what to fix. If the folder placement seems off, we'll suggest a move. Assets won't be rejected on aesthetic grounds.

Once merged, assets sit in `open/`. Over time, well-used and high-quality assets move into `curated/` — contributors don't need to track this.

---

## Other contributions

Found a broken link or something wrong in the documentation? Open an issue or submit a PR directly.

Questions? Open an issue and ask.
