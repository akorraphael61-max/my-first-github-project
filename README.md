# my-first-github-project

A simple personal homepage and learning project by Akor Raphael. This repository contains a small static site used to practice HTML, CSS, and GitHub Pages.

## What’s in this repository

- `index.html` — the site homepage (project root).
- `css/style.css` — site styles.
- `assets/images/` — images used by the site (add your images here).

## About

This project is a beginner-friendly portfolio/playground for learning web development and GitHub. The contact form in `index.html` is for demonstration and does not send messages until a form handler (backend) or a form service (e.g., Formspree or Netlify Forms) is configured.

## Quick start (local preview)

1. Clone the repo:

   git clone https://github.com/akorraphael61-max/my-first-github-project.git
   cd my-first-github-project

2. Start a simple HTTP server and open the site in your browser:

   python3 -m http.server 8000
   # then open http://localhost:8000

Or open `index.html` directly in your browser.

## Publish with GitHub Pages

1. Make sure `index.html` is at the repository root on the branch you want to publish (default branch is `main`).
2. In GitHub: go to Repository → Settings → Pages → Build and deployment. Select:
   - Branch: `main`
   - Folder: `/ (root)`
3. Save. The site will be available at:

   https://akorraphael61-max.github.io/my-first-github-project/

Give it a minute to build after you enable Pages.

## Replace placeholders

- Images: The current site uses a placeholder image. Add your images to `assets/images/` and update the `<img>` `src` in `index.html`.
- Email/contact: Replace the placeholder contact email in `index.html` with your email or configure a form service to handle submissions.

Example: Use Formspree (no backend required)

1. Create a free Formspree form at https://formspree.io/ and note the form endpoint (looks like `https://formspree.io/f/your-id`).
2. In `index.html` update the `<form>` tag to:

   <form action="https://formspree.io/f/your-id" method="POST">
     <!-- your inputs -->
   </form>

3. Optionally add a hidden input to prevent spam or to set a redirect after submit (example in `index.html` uses `_next` to redirect to a thank-you page).

I can help add a working Formspree example if you want — tell me your Formspree form ID or I can add a placeholder action and instructions.

## Screenshot / Demo

![Site screenshot](https://via.placeholder.com/800x400?text=Site+Screenshot)

Visit the live demo (after enabling Pages):

https://akorraphael61-max.github.io/my-first-github-project/

There is also a simple `thank-you.html` page included that the form can redirect to after a successful submit. To enable the redirect with Formspree, add this hidden input to your form (already included in the example form in `index.html`):

```html
<input type="hidden" name="_next" value="https://akorraphael61-max.github.io/my-first-github-project/thank-you.html">
```

## Accessibility & responsiveness checklist

- Add viewport meta to `index.html` head: `<meta name="viewport" content="width=device-width,initial-scale=1">`.
- Use semantic HTML elements (header, nav, main, footer) for structure.
- Add meaningful `alt` text for images.
- Check color contrast for legibility (tools: WebAIM contrast checker).
- Ensure the site scales on mobile (flexbox/grid, relative units, media queries).

## Recommended repo housekeeping

- LICENSE: Add a license file if you want to publish the project under a specific license (MIT is common for personal projects).
- .gitignore: Add common ignores such as `.DS_Store`, `node_modules/` (if you add Node), and editor temp files.
- Screenshots: Add a `screenshot.png` or `demo.gif` at the repo root and reference it in the README to show what the site looks like.
- CI (optional): Add a basic GitHub Actions workflow to run HTML/CSS linters or link checkers on push.

## Notes

- Pull Request #3: A previous PR mixed HTML/CSS into `README.md`, which made the repository messy. Keep site files in `index.html` and `css/style.css` and do not merge HTML directly into README.

## How to contribute

1. Create a new branch for your change:

   git checkout -b feature/your-change

2. Make changes, commit, and open a pull request describing the change.

3. I recommend including a screenshot or short description in the PR for UI changes.

## License

This project is published under the MIT License. See the `LICENSE` file for details.

---

If you want more changes I can:
- Wire the contact form to Formspree (add your Formspree ID) — I can update the form action and add a redirect.
- Replace the avatar image with a real photo you provide (add the image to `assets/images/`).
- Add a real screenshot file and update README to use it.
