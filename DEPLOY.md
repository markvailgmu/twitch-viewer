# Deploy Twitch Viewer (any network)

Twitch embeds only work when the page is served over **HTTPS** from a **real domain** (not a raw LAN IP). GitHub Pages, Netlify, and Cloudflare Pages are free and work from phone data, Wi‑Fi, or anywhere.

## Option A: GitHub Pages (recommended)

1. **Create a new repository** on GitHub (e.g. `twitch-viewer`). It can be public or private (GitHub allows private repos with Pages on paid plans; public repos get free Pages).

2. **Upload these files** to the repo root (or clone locally and push):
   - `twitch-viewer.html`
   - `index.html` (optional shortcut to the viewer)

3. **Enable Pages**
   - Repo **Settings** → **Pages**
   - **Source**: Deploy from a branch
   - **Branch**: `main` (or `master`), folder **/ (root)**
   - Save

4. After a minute, your site will be at:
   - **User site:** `https://YOUR_USERNAME.github.io/REPO_NAME/`
   - Open `https://YOUR_USERNAME.github.io/REPO_NAME/twitch-viewer.html`  
     or the root URL if you added `index.html`.

5. **Twitch parent domain** is filled automatically (`YOUR_USERNAME.github.io`). Embeds should work on any network.

## Option B: Netlify Drop

1. Go to [https://app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the folder containing `twitch-viewer.html` (and `index.html` if you use it).
3. You get a random `something.netlify.app` URL — that domain is valid for Twitch embeds.

## Option C: Cloudflare Pages

Connect the same GitHub repo to Cloudflare Pages; you get a `*.pages.dev` URL that also works as a Twitch parent.

---

**Note:** Do not commit secrets in HTML; this app has none. If you use a **custom domain**, set the “Hosting domain” field on the page to your custom hostname once, or rely on auto-detection from `location.hostname`.
