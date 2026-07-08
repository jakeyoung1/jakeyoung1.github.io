# Jake Young · Portfolio

Single-page portfolio. Static HTML + CSS, no framework, no build step, no JavaScript.

## Files

- `index.html` : the whole site
- `styles.css` : all styling ("Scorecard" design: cream paper, green ink, red stamp)
- `assets/Jake_Young_Resume.docx` : downloadable resume (keep in sync with `~/Desktop/jake_young_resume_FINAL.docx`)
- `PRODUCT.md` : design/product brief the site was built against

## Preview locally

```bash
cd portfolio
python3 -m http.server 8080
# open http://localhost:8080
```

## Deploy to GitHub Pages (free, ~2 minutes)

```bash
cd portfolio
git init && git add -A && git commit -m "Portfolio"
gh repo create jakeyoung1.github.io --public --source=. --push
```

Repo named `jakeyoung1.github.io` publishes automatically at **https://jakeyoung1.github.io** within a minute or two (Settings > Pages should show "main / root" as source).

Then put that URL on the resume header, LinkedIn, and GitHub profile.

## Updating

Edit `index.html`, replace the resume file in `assets/`, commit, push. Pages redeploys automatically.
