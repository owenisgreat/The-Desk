# The Desk — setup & deployment

## What's in here
- `index.html` — homepage listing all your pitches with BUY/WATCH/PASS ratings
- `style.css` — shared styling for the whole site
- `pitches/template.html` — blank memo template (matches your investment memo format: overview, thesis, catalysts, risks, competitive landscape, macro context, horizon/sizing, key metrics)
- `pitches/example-pitch.html` — a copy of the template, ready to fill in as your first real pitch

## Publish it with GitHub Pages (no build tools needed)

1. Create a new repo on GitHub (e.g. `the-desk`), or use your existing one.
2. Upload these files, keeping the folder structure (`index.html` and `style.css` at the root, `pitches/` as a subfolder).
3. In the repo: **Settings → Pages → Source** → select the `main` branch, root folder → Save.
4. GitHub gives you a URL like `https://yourusername.github.io/the-desk/` — that's your live site, usually live within a minute or two.

## Adding a new pitch each week
1. Duplicate `pitches/template.html`, rename it something like `pitches/company-name.html`.
2. Fill in the bracketed placeholders.
3. Open `index.html`, copy one `<li class="pitch-row">...</li>` block, update the rating class (`buy`, `watch`, or `pass`), link text, href, and date.
4. Commit and push — GitHub Pages updates automatically.

No build step, no dependencies — just plain HTML/CSS files you edit directly and push.
