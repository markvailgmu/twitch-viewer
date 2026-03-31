# Finish pushing to GitHub (one time)

Your local repo is ready. The remote `markvailgmu/twitch-viewer` must exist on GitHub first.

## Step 1 — Create the empty repo

1. Open: **https://github.com/new?name=twitch-viewer**
2. Set **Repository name** to: `twitch-viewer`
3. Choose **Public**
4. Do **not** add README, .gitignore, or license (keep it empty)
5. Click **Create repository**

## Step 2 — Push from this folder

In PowerShell:

```powershell
cd "c:\Users\fuzzy\Music\hw9"
git push -u origin main
```

Sign in to GitHub if prompted (browser or Personal Access Token).

## Step 3 — Turn on GitHub Pages

1. Repo **Settings** → **Pages**
2. **Source**: Deploy from a branch
3. **Branch**: `main`, folder **/ (root)** → Save

After ~1 minute your site will be:

**https://markvailgmu.github.io/twitch-viewer/**

Open `twitch-viewer.html` or use the root URL (redirects via `index.html`).
