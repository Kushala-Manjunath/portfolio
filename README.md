# Portfolio & Resume Workspace

This repository contains a static portfolio site and a LaTeX-based resume workflow designed for quick iteration and GitHub Pages deployment.

## Project Structure

- `portfolio/` — Static site assets (HTML, CSS, JS, images, resume PDF).
- `resume/` — LaTeX source for the resume and workflow notes.
- `portfolio/assets/resume/` — Place the compiled `resume.pdf` here; the site links reference this path.

## Getting Started

1. Customize `portfolio/index.html`, `portfolio/css/styles.css`, and `portfolio/js/main.js` with your biography, projects, and contact links.
2. Update `resume/resume.tex` with your experience. Compile it with `pdflatex resume.tex` (from within the `resume/` folder) to produce `resume.pdf`.
3. Move the compiled `resume.pdf` to `portfolio/assets/resume/resume.pdf`.

## Local Preview

Open `portfolio/index.html` directly in your browser, or serve it via a lightweight HTTP server:

```bash
cd portfolio
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploying to GitHub Pages

1. Create a new GitHub repository and push this project.
2. In the repository settings, enable GitHub Pages and set the source to the `main` branch with the `/portfolio` folder.
3. GitHub Pages will serve the site at `https://<username>.github.io/<repository>/` within a few minutes.

Whenever you update your portfolio or resume, rebuild `resume.pdf`, move it into `portfolio/assets/resume/`, commit the changes, and push to GitHub.
