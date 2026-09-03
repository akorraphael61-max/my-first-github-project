# my-first-github-project

A simple personal homepage and learning project by Akor Raphael. This repository contains a small static site used to practice HTML, CSS, and GitHub Pages.

## What’s in this repository

- `index.html` — the site homepage (project root).
- `css/style.css` — site styles.
- `assets/images/` — images used by the site (add your images here).

## About

This project is a beginner-friendly portfolio/playground for learning web development and GitHub. The contact form in `index.html` is for demonstration and does not send messages until a form handler or third-party service is configured.

## Local preview

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
   `https://akorraphael61-max.github.io/my-first-github-project/` (give it a minute to build).

## Notes

- Placeholders: The current site uses a placeholder image and a placeholder contact email. Replace them in `index.html` with your own image (put files under `assets/images/`) and your email.
- Contact form: To make the form work without a backend, use services like Formspree or Netlify Forms. I can add a Formspree configuration if you want.
- Pull Request #3: This PR mixes HTML/CSS into `README.md`, which would make the repository messy. Do not merge that PR as-is. The site files have been placed properly in `index.html` and `css/style.css` instead.

## How to contribute

1. Create a new branch for your change:

   git checkout -b feature/your-change

2. Make changes, commit, and open a pull request.

## License

Add a license file if you want to publish this project with specific terms.
