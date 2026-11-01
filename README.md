# Blue Grit website

Standalone static recreation of https://bandsites.my.canva.site/blue-grit, retrieved 1 November 2026. Contains the original introduction, member biographies, contact copy, photographs, banner and emblem, with responsive layouts. The only copy correction is a missing space in Ian's biography.

## Publish on GitHub Pages

1. Create a new **public** GitHub repository named `bluegrit-site`. Do not reuse `bandmade-pages`: GitHub Pages supports only one custom domain per repository.
2. Upload the CONTENTS of this folder into the repository root: `index.html`, `styles.css`, `assets/`, `CNAME`, and `.nojekyll`. Do not upload the ZIP itself. The README is optional. The hidden `.nojekyll` file is optional for this buildless site.
3. In repository **Settings > Pages**, choose **Deploy from a branch**, branch **main**, folder **/(root)**, and Save.
4. Set the custom domain to `bluegrit.bandmade.au` and Save.
5. At your DNS provider, add a CNAME for host/name `bluegrit` targeting `iand2124-arch.github.io`. Use the hostname only, without `https://` or a repository path. Resolve any existing conflicting records for `bluegrit` only; preserve the other domain records, including `bandapp`.
6. After GitHub's DNS check succeeds and its certificate is issued, enable **Enforce HTTPS**.

The included CNAME file already contains `bluegrit.bandmade.au`. Set up the GitHub custom domain before adding its DNS record. DNS and HTTPS issuance may take time.

## Local preview

Open `index.html` in a web browser. For a local web server, run `python -m http.server 8080` inside this folder, then visit http://localhost:8080.

## Editing

All copy is in `index.html`; layout and fonts are in `styles.css`. Images and font files are local in `assets/`. There is no build step, framework, external Canva runtime, or tracking script. Edits to the original Canva design will not automatically update this independent website.

The Facebook and Instagram icons in the source Canva design had no destination URLs. They remain labelled images here. Add the verified profile links to `index.html` when available. The email link works.

## Validation

Checked local HTML/CSS asset paths, image file integrity, CNAME and canonical domain. Browser visual verification could not run in the creation session; check desktop and phone appearance before launch.
