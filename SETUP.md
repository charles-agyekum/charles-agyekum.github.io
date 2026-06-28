# SETUP — GitHub Pages

The site is **already live** at **https://charles-agyekum.github.io** (username
`charles-agyekum`, repo `charles-agyekum.github.io`, branch `main`). This file is
kept as a reference. For day-to-day changes you only need the "Updating" steps below.

---

## Updating the site (the normal case)

Open a terminal **inside this `Portfolio_Site` folder** and run:

```bash
git add -A
git commit -m "Describe the change"
git push
```

GitHub Pages redeploys automatically within a minute or two. Refresh
`https://charles-agyekum.github.io` to see it.

If git asks you to sign in, use your GitHub username (`charles-agyekum`) and a
**personal access token** as the password (not your account password). Create one at:
GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic) →
Generate new token, tick the `repo` scope, copy it, and paste it when prompted.

## Pages configuration (already set, for reference)

- Repo **Settings → Pages → Build and deployment**
- Source: **Deploy from a branch**
- Branch: **main**, folder: **/ (root)**

This site is plain HTML, so a `.nojekyll` file tells Pages to serve the files as-is
without trying to run a Jekyll build. Leave that file in place.

## One-time setup (already done)

Recorded here only in case the repo is ever recreated from scratch:

```bash
git init
git add .
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/charles-agyekum/charles-agyekum.github.io.git
git push -u origin main
```

## Optional, when you want it

- **Add the workbook files for download.** The `.xlsx` and `.pbix` files are large and
  not in the repo. To let visitors download them, drop the files into `assets/files/`
  and add a link on the relevant project page.
- **Contact details.** The contact email on the landing page is set in `index.html`
  (search for `mailto:`). Update it there if it changes.
