# Badru Olumide David — Developer Portfolio

A responsive, static portfolio with selected software projects, project notes, experience, a downloadable résumé and a contact form.

## Preview

From this directory, run:

```sh
python3 -m http.server 8000
```

Open `http://localhost:8000`. No package installation or build step is required.

## Pages and assets

- `index.html`: introduction, selected projects, skills, experience and contact.
- `projects.html`: more detailed project notes; existing page URL is preserved.
- `assets/css/portfolio.css`: layout, typography, responsive rules and reduced-motion support.
- `assets/js/portfolio.js`: mobile navigation and contact-form feedback.
- `assets/documents/Badru_Olumide_David_Developer_Resume.pdf`: downloadable developer résumé.
- `assets/images/`: favicon and losslessly compressed WebP screenshots for Gataama and Honest Scholars.

Content is available without JavaScript. External project links open in a new tab. The résumé is a local PDF download.

## Updating the portfolio

Edit project summaries in `index.html` and the corresponding notes in `projects.html`. Keep contribution descriptions and project status accurate. GradeVault is currently marked **in development**; add a public demo link only after it is deployed. Its private source repository is intentionally not linked.

Replace the PDF at the same path when updating the résumé. Both pages link to this file.

The contact form retains the existing Formspree endpoint. Without JavaScript it submits directly to Formspree; with JavaScript it displays confirmation only after a successful response and preserves the message when delivery cannot be confirmed. The email link provides a fallback. Do not submit synthetic test messages to the live endpoint without the owner's permission.

## Deployment

This repository is a plain static site. It can be published from the repository root on Netlify, with no build command. Review any existing Netlify build and publish settings before changing them. The canonical URL remains `https://badrudavidportfolio.netlify.app/`.

Review the refresh on its branch or a deploy preview before merging into the production branch.

## Performance and legacy template

The current pages load one small stylesheet and one deferred JavaScript file. They use system fonts, and both project screenshots are lazy-loaded, losslessly compressed WebP files with explicit dimensions. The résumé is downloaded only when requested.

Unused template stylesheets, Sass sources, jQuery plugins, icon fonts, old gallery images and the unrelated Android APK have been removed. The previous site used HTML5 UP's Big Picture template; its original `LICENSE.txt` is retained for attribution and historical context. Earlier code and assets remain available in Git history.
