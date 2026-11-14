# INF2005 Study & Revision Playbook — GitHub Pages edition

A React + TypeScript + Vite app with notes, a question bank, quizzes and local browser progress.

## Deploy
1. Create a **public** GitHub repository named `INF2005-Study-Playbook`.
2. Upload the **contents of this folder** (including `.github/workflows/deploy.yml`) to the repository root. GitHub's web upload may hide dot-folders on some systems; check that `.github/workflows/deploy.yml` is committed.
3. In GitHub: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
4. Open the **Actions** tab and wait for the Deploy to GitHub Pages workflow to finish.
5. Visit `https://YOUR_USERNAME.github.io/INF2005-Study-Playbook/`.

To change the repository name, update `base` in `vite.config.ts` to `/<new-repository-name>/`.

## Local development
```bash
npm install
npm run dev
```

## Notes
- The original lecture PDFs are excluded to keep the download small and avoid publicly redistributing teaching materials. Citations remain visible as filename and page number, but PDF links are disabled.
- Quiz progress uses localStorage (per browser/device, not synchronized).
- This is an initial content build with a limited question bank, not complete coverage of all lectures. Some quiz formats may have no matching questions.
