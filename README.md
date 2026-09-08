# yujinn-k.github.io

Personal academic homepage of Yujin Kim, served with GitHub Pages at
<https://yujinn-k.github.io>.

Plain HTML + CSS, no build step, no JavaScript beyond a one-line image fallback.

## Structure

```
yujinn-k.github.io/
├── index.html          # page content
├── style.css           # styling
├── README.md
├── .nojekyll           # tells GitHub Pages to serve files as-is
└── assets/
    ├── profile.jpeg         # (add) profile photo, ~300x300 px, square
    └── Yujin_Kim_CV.pdf    # (add) CV
```

## Files to add manually

| What | Where | Notes |
|---|---|---|
| Profile photo | `assets/profile.jpeg` | Square image, ~300×300 px. If missing, the photo is simply hidden. |
| CV | `assets/Yujin_Kim_CV.pdf` | The "CV" link already points here. |

## Deploying to GitHub Pages

1. Create a **public** repository named exactly `yujinn-k.github.io` on GitHub
   (the name must match your username for the root URL to work).
2. Push this folder to the `main` branch:

   ```bash
   cd yujinn-k.github.io
   git init
   git add .
   git commit -m "Initial academic homepage"
   git branch -M main
   git remote add origin https://github.com/yujinn-k/yujinn-k.github.io.git
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch `main`, folder `/ (root)`. Save.
4. After a minute or two the site is live at <https://yujinn-k.github.io>.

Updating later:

```bash
git add .
git commit -m "Update news"
git push
```

## Local preview

Open `index.html` directly in a browser, or run
`python3 -m http.server 8000` in this folder and visit <http://localhost:8000>.
