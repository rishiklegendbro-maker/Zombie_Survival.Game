Zombie Survival.Game — GitHub Pages deployment

A mobile-first zombie shooter that runs in a phone browser.

Recommended repo description:
- Mobile-only browser zombie shooter — play on your phone.

This folder is a ready-to-upload site for publishing your local game using GitHub Pages.

Files to include in the repo root:
- `index.html`  (this redirect page)
- `Zombie Survival.html`  (your full game file — keep the exact filename or update the redirect)
- `Zombie Survival Link.html` (optional)

Quick publish steps (GitHub web UI):
1. Create a new GitHub repository (e.g. `zombie-survival-game`).
2. Upload `index.html` and `Zombie Survival.html` to the repository root using the "Add file → Upload files" button.
3. Commit the changes.
4. In the repository Settings → Pages, choose branch `main` (or `master`) and folder `/ (root)`, then Save.
5. After a minute the site will be available at `https://<your-username>.github.io/<repo>/` — opening that URL loads `index.html` and redirects to the game.

Publish via git (command line):

```bash
# from this folder (on your PC)
git init
git add .
git commit -m "Initial site with Zombie Survival"
# create a repo on GitHub (or use existing) then:
git branch -M main
git remote add origin https://github.com/<your-username>/<repo>.git
git push -u origin main
```

Notes:
- If you prefer a nicer filename, rename `Zombie Survival.html` to `zombie-survival.html` and update the redirect in `index.html`.
- GitHub Pages is free and simple for static HTML. Alternatives: Netlify, Vercel, or any static host.
- Once hosted, your public URL can be shared and opened from any phone browser; Google indexing is separate but optional.
