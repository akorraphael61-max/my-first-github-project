# my-first-github-project

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE) [![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Enabled-green.svg)]

A small personal homepage and learning project by Akor Raphael. This static site is a beginner-friendly portfolio and playground for practicing HTML, CSS, accessibility, and GitHub Pages.

Live demo
https://akorraphael61-max.github.io/my-first-github-project/ (enable GitHub Pages on the main branch if not already active)

---

## Table of contents
- About
- Features
- Quick start
- Run locally
- Contact form (Formspree)
- Accessibility & responsiveness
- Repo housekeeping
- Contributing
- License
- Contact

## About
This project is a minimal personal site that demonstrates:
- Basic HTML/CSS layout and styling
- A simple contact form with optional Formspree integration
- Accessibility improvements (skip link, focus styles, aria-live feedback)
- Ready-to-deploy structure for GitHub Pages

## Features
- `index.html` — homepage (root)
- `css/style.css` — styles with responsive and accessibility enhancements
- `assets/images/` — place your images here (avatar, screenshots)
- Client-side contact form demo fallback while the Formspree ID is a placeholder
- `thank-you.html` and `privacy.html` included for form redirect and privacy info
- Basic CI workflow (`.github/workflows/validate.yml`) to check key files

## Quick start
Clone this repository and preview locally:

```bash
git clone https://github.com/akorraphael61-max/my-first-github-project.git
cd my-first-github-project
```

## Run locally
Start a simple static server (Python):

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Publish with GitHub Pages
1. Ensure `index.html` is at the repository root on the branch you want to publish (default branch is `main`).
2. In GitHub: Repository → Settings → Pages → Build and deployment.
   - Branch: `main`
   - Folder: `/ (root)`
3. Save. Your site will be available at:

https://akorraphael61-max.github.io/my-first-github-project/ (allow a minute to build)

## Contact form (Formspree)
The contact form uses a placeholder action by default:

```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST"> ... </form>
```

Demo behavior: while the placeholder ID remains, the site uses a client-side fallback that displays a local “Sent” message (no external request).

To enable real submissions:
1. Create a free form at https://formspree.io/ and copy the form endpoint (looks like `https://formspree.io/f/xxxxxx`).
2. Replace `YOUR_FORM_ID` in `index.html` with your real endpoint.
3. (Optional) Keep the included redirect to the thank-you page:

```html
<input type="hidden" name="_next" value="https://akorraphael61-max.github.io/my-first-github-project/thank-you.html">
```

Privacy & consent: the form includes a consent checkbox and a honeypot field. See `privacy.html` for details.

## Accessibility & responsiveness checklist
- meta viewport is included for mobile devices.
- Skip-to-content link for keyboard users.
- Focus-visible styles and accessible form elements with ARIA where useful.
- Responsive layout and larger touch targets for mobile.

## Repo housekeeping suggestions
- LICENSE: MIT (already added). Link included above.
- .gitignore: includes common ignores (.DS_Store, node_modules, .env, editor folders).
- Replace placeholder images: add your avatar to `assets/images/` and update `index.html`.
- Add a real screenshot to the README (place `screenshot.png` at the repo root).
- Enhance CI: add link-checker or HTML/CSS validation steps to `.github/workflows`.

## Contributing
1. Fork or create a branch: `git checkout -b feature/your-change`
2. Make changes, commit, and open a pull request.
3. Include a screenshot for UI changes and a short description of the change.

## License
This project is published under the MIT License. See `LICENSE` for details.

---

If you want me to commit this polished README.md, reply “Confirm” and I’ll update the file in the repository. If you want edits (tone, badges, add social links), reply “Edit” and tell me what to change.