```markdown
# hire me — changement de carrière (Julius Gruebl)

This repo contains a single page to present Julius Gruebl's CV and two YouTube videos (short + longer intro).

Files to include in the repository root:
- index.html  (the page)
- cv.pdf      (your actual CV file — name it exactly `cv.pdf`)

What I included
- Embedded short video (YouTube ID: po2kqdABvOA).
- Embedded longer video (YouTube ID: R0CGgLYGQ6M).
- Two CV actions: "Voir le CV (nouvel onglet)" and "Télécharger le CV".
- Contact mailto: juliuscuisine@posteo.com

Local testing
1. Put index.html and cv.pdf in a folder.
2. Start a simple HTTP server so the PDF link behaves correctly:
   - Python 3: `python -m http.server 8000`
   - OR (Node): `npx serve` (if you have Node)
3. Open in your browser: http://localhost:8000

Publish on GitHub Pages
1. Create a new repository on GitHub named `hire-me` under your account `juliusgruebl-ctrl`.
   - Make it Public (so Pages serves it) or keep it Private and use another public repo for the site.
   - You can create the repo via https://github.com/new.

2. From the project folder run these commands (exact):
```bash
git init
git add index.html README.md cv.pdf
git commit -m "Initial site: hire me — changement de carrière"
git branch -M main
# SSH
git remote add origin git@github.com:juliusgruebl-ctrl/hire-me.git
# or HTTPS:
# git remote add origin https://github.com/juliusgruebl-ctrl/hire-me.git
git push -u origin main
```

3. Enable GitHub Pages:
   - On GitHub, open the repo → Settings → Pages (or "Pages" in the left sidebar).
   - Under "Build and deployment" set Source to: Branch = main, Folder = / (root).
   - Save. After a short delay the site will be available at:
     `https://juliusgruebl-ctrl.github.io/hire-me/`

4. Verify:
   - Visit the published URL and confirm videos play and the CV link opens/downloads `cv.pdf`.
   - If the PDF doesn't show, ensure cv.pdf exists in repo root and the filename matches exactly.

Notes & privacy
- cv.pdf will be publicly accessible if the repo is public.
- If you prefer not to publish the CV publicly, either:
  - Remove cv.pdf from the repo and host it privately, linking to it manually when needed, or
  - Make the repo private and deploy only the static site to a separate public repo.

If you want me to push the files for you
- I attempted to create/access the repository but couldn't because it doesn't exist under your account (or I lack access). I can push if you either:
  1) Create an empty repo named `hire-me` under your account (no README needed), then tell me and I will push; OR
  2) Give me the repo URL and confirm you want me to push into an existing repo (I will then proceed).
```