# Ruth Sharon's portfolio

GitHub Pages serves `index.html` from the root of `main`.

- `index.html`: the latest portfolio export, page content, and navigation.
- `support.js`: dependency-free DOM bindings so the exported template runs on GitHub Pages.
- `about.css`: the reference-matched About layout and small-screen styles.
- `assets/about-reference.png`: the supplied design reference, displayed through SVG viewports for the original photos and social icons. This keeps the supplied pixels unchanged; replace the photo viewports with original photo files when available.
- `notindex.html`: the previous export, retained as an archive.

To preview locally, run `python -m http.server 8765` and open `http://localhost:8765/#about`.

The About page's resume link requests the resume by email because no resume PDF was included. Interests and project entries retain the latest export's existing content and image placeholders. Font files referenced by the export were absent, so the site uses available fallback fonts; About uses Arial/Helvetica.

Deploy by committing changes to `main`. In GitHub Settings → Pages, select **Deploy from a branch**, **main**, and **/(root)**. The `pages build and deployment` action reports publication status. Direct links such as `#about`, `#interests`, and `#lab` support reloads and browser back/forward navigation.
