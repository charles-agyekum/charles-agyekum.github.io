# SETUP — publish this site on GitHub Pages

Account done. Username: **charles-agyekum**. Your site will go live at:

**https://charles-agyekum.github.io**

Everything in this folder is pre-filled for that username. Work top to bottom.

---

## Step 1 — Create the repository

1. Click the **+** top right, then **New repository**.
2. Repository name: type it **exactly** as `charles-agyekum.github.io`. GitHub will
   show a note confirming it recognises this as a Pages site. That note is how you
   know the name is right.
3. Set it to **Public**.
4. Do **not** tick "Add a README" (this folder already has one).
5. Click **Create repository**.

## Step 2 — Push the files

Open a terminal **inside this `Portfolio_Site` folder** and run these in order.

```bash
git init
git add .
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/charles-agyekum/charles-agyekum.github.io.git
git push -u origin main
```

If git asks you to sign in, use your GitHub username (`charles-agyekum`) and a
**personal access token** as the password (GitHub no longer accepts your account
password here). Create one at: GitHub → Settings → Developer settings → Personal
access tokens → Tokens (classic) → Generate new token, tick the `repo` scope, copy
it, and paste it when prompted.

> No git installed? Download it from https://git-scm.com/download/win, accept the
> defaults, then reopen the terminal and run the commands above. If you would
> rather avoid the command line entirely, tell me and I will write you the
> GitHub Desktop (point-and-click) version instead.

## Step 3 — Turn on Pages

1. In the repo, go to **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Branch: **main**, folder: **/ (root)**. Save.
4. Wait one to two minutes. The page will show your live URL:
   `https://charles-agyekum.github.io`.

## Step 4 — Check it

Open `https://charles-agyekum.github.io`. You should see the landing page with the
six project links. Click into one to confirm the project pages load.

Done means: repo created, files pushed, Pages on, live URL working. Tell me when it
is live and I will log it to PROGRESS.md and move the Command Center bar.

---

## Optional, when you want it

- **Add the workbook files for download.** The `.xlsx` and `.pbix` files are large
  and are not copied in yet. If you want visitors to download them, copy the files
  into `assets/files/` and I will wire the links. (The `.gitignore` ignores raw
  `.csv` on purpose, so source data is referenced, not republished.)
- **DataCo page.** Once Saturday's build is done, I will add its project page and
  link it on the homepage. That is the differentiated centrepiece.
- **Contact details.** Add your email and LinkedIn in `_config.yml` and I will
  surface them on the landing page.
