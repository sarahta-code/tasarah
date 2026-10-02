# Editing this site

Everything lives in `index.html`. Open it in any text editor (VS Code, Sublime, even
Notepad) or edit it directly on GitHub in the browser. Assets sit in `assets/`.

## The Work section

Each box in Work is one `<article class="case" ...>`. There are three:

| Box | Search for |
|---|---|
| Operating room turnover (Stanford) | `Cutting operating room turnover` |
| HP startup evaluation | `Evaluating startups` |
| Design and video work | `id="design"` |

To reorder them, cut a whole `<article>...</article>` block and paste it above or below
another one.

Every box has the same four parts, top to bottom:

1. **Title** (`case-title`) and a **result line** (`case-hook`), the one-line result
   shown when the box is closed.
2. **Chips** (`case-tags`): the category chips, plus a grey one for the organization.
3. **Description**: one or two sentences, right under the divider.
4. **Result tiles** (`class="stats"`): a big number and a short label. To add one, copy a
   line like `<li><b>37,700</b><span>OR minutes recovered...</span></li>`.

Then the evidence (video, memo pages, posters).

The filter buttons at the top of Work read each box's `data-tags`. Use `product`,
`analysis`, or `creative`. To add another case study, copy an existing `<article>` block,
give its button and body a new matching `c5` / `aria-controls` id, and set `data-tags`.

## Design and video box

### Adding a design

Save it as `assets/design-10.jpg`, then copy one `<button class="gal-item">` line inside
`<div class="gallery" id="gallery">` and change the filename and the `alt` text.

Then update the count under the collapsed box: search for `peek-count` and change
"8 designs and 3 videos". The little fanned stack on the collapsed box uses the first five
images; to change which ones, search for `peek-stack`.

### Adding a video

Copy one `<div>` block inside `<div class="vid-grid">`, then change the thumbnail path and
both Drive URLs (the card link and the caption link). Update `peek-count` too.

### Captions

Search for `gal-note`.

## Other common edits

| What | Search for |
|---|---|
| Email address | `sarahta@ucla.edu` |
| LinkedIn URL | `linkedin.com/in/tasarah` |
| Hero tagline | `class="thesis"` |
| About blurb | `class="about-body"` |
| Nav links | `var NAV` |
