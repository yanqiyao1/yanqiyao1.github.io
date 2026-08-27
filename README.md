# Qiyao Yan — Academic Homepage

Pure static personal academic homepage (HTML/CSS/JS, no build step).
Live at: https://yanqiyao1.github.io (once deployed).

## Local preview

```bash
cd resume
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a **public** repository named `yanqiyao1.github.io` on GitHub.
2. In this directory:

   ```bash
   git init
   git add .
   git commit -m "Initial academic homepage"
   git branch -M main
   git remote add origin git@github.com:yanqiyao1/yanqiyao1.github.io.git
   git push -u origin main
   ```

3. In the repo: **Settings → Pages → Source: Deploy from a branch → main / (root)**.
   The site will be live at `https://yanqiyao1.github.io` within a minute.

(Or use the GitHub CLI: `gh repo create yanqiyao1.github.io --public --source . --push`.)

## Updating content

- All content lives in `index.html` (sections: About / News / Publications / Projects / Education).
- Photo: replace `assets/headshot.jpg`.
- Papers: put PDFs in `assets/papers/` and link them in the publication entries.
- Replace the `Google Scholar` / `CV` placeholder links once available.
