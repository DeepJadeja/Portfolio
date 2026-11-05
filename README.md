# Chandradeepsinh (Jade) Jadeja — Portfolio

A small, fast, dependency-free static site. Pure HTML + CSS (fonts from Google Fonts).
No build step, no framework — just open or deploy the files.

## Pages
- `index.html` — landing (block grid)
- `work.html` — experience + projects
- `skills.html` — tools + stack
- `about.html` — about + education
- `connect.html` — contact

All links are relative, so it works on any static host.

## Run locally
Just open `index.html` in a browser. (For clean navigation you can also run a tiny
local server: `python -m http.server` then visit http://localhost:8000 )

## Deploy — pick ONE

### Option A — GitHub Pages (free, uses your repo)
1. Create a new repo on GitHub (e.g. `portfolio`).
2. Push this folder (see "Push to git" below).
3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch **main**, folder **/ (root)**, then **Save**.
4. Your site goes live at `https://<your-username>.github.io/portfolio/` in ~1 minute.

### Option B — Netlify (free, drag-and-drop, custom domain easy)
1. Go to https://app.netlify.com/drop
2. Drag this whole folder onto the page.
3. It's live instantly at a `*.netlify.app` URL you can rename.

### Option C — Vercel (free)
1. Push to GitHub (below), then import the repo at https://vercel.com/new
2. Framework preset: **Other**. Deploy. Done.

## Push to git
Run these from inside this folder:

```
git init
git add .
git commit -m "Portfolio site"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

## Custom domain (optional)
Netlify and Vercel both let you add a domain under the project's Domain settings.
GitHub Pages: add a `CNAME` file with your domain and set DNS at your registrar.
