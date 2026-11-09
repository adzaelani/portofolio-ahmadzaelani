# .NET Developer Portfolio — Tailwind CSS v4

Responsive one-page portfolio inspired by the reference website's information architecture: Home, About, Tech Stack, Projects, Education, Experience, Blog, Contact. It uses an original visual design and your .NET career information.

## Features
- Tailwind CSS v4 compiled with the CLI (no CDN runtime)
- Light/dark toggle, remembers preference in localStorage
- Uses operating-system theme on first visit
- Responsive navigation and mobile menu
- Static website; no backend or database

## Run/build
Requires Node.js and npm.

```bash
npm install
npm run build
```

For local preview, use a static server such as `npx serve .`. During editing use `npm run watch`.

## Customize before publishing
Replace in `index.html`:
- `[Your Name]`
- `[Company Name]`, `[Month Year]`
- `[Degree / Major]`, `[University / Institution]`, `[Graduation Year]`
- `your.email@example.com`
- `YOUR-USERNAME`, `YOUR-LINKEDIN`

Optional: put your CV at `assets/cv.pdf` or remove the Download CV link if you do not have a PDF yet. Replace blog idea cards with actual articles when published. Verify all skills and experience statements. Do not publish confidential company screenshots, source code, case records, credentials, or proprietary details.

## Publish on GitHub Pages
Recommended: use the included GitHub Actions workflow.
1. Create a public repository named `YOUR-USERNAME.github.io` (or use a project repository).
2. Push the project files to the `main` branch.
3. Open **Settings → Pages** and set Source to **GitHub Actions**.
4. Push to `main`; Actions installs Tailwind, builds `dist/output.css`, then deploys the static site.

The CSS output is built in CI. For branch-based Pages deployment instead, run `npm install && npm run build` locally and commit `dist/output.css` before choosing `main` / `/(root)` in Pages settings.

The relative CSS path (`./dist/output.css`) works on both user and project pages.
