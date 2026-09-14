# Brayan695.github.io

Personal academic website for Brayan Gutierrez — built as a static site (plain HTML/CSS/JS, no build step).

## What's here

- `index.html` — the whole site (About, Education, Research Experience, Projects & Repositories, Publications, Honors, Skills, Contact)
- `assets/style.css` — styling
- `assets/script.js` — mobile nav toggle + footer year
- `assets/Brayan_Gutierrez_CV.pdf` — downloadable CV (linked from the site)

## Deploy to GitHub Pages

This repo is already named `Brayan695.github.io`, which GitHub Pages treats specially — once pushed, it's served automatically at:

```
https://brayan695.github.io
```

Steps:

1. Create a new **empty** repository on GitHub named exactly `Brayan695.github.io` (no README, no .gitignore — this folder already has its own).
2. From this folder, push it:

   ```bash
   git remote add origin https://github.com/Brayan695/Brayan695.github.io.git
   git branch -M main
   git push -u origin main
   ```

3. In the repo's **Settings → Pages**, set the source to `Deploy from a branch`, branch `main`, folder `/ (root)` (GitHub usually detects and enables this automatically for a `<username>.github.io` repo).
4. Wait 1–2 minutes, then visit `https://brayan695.github.io`.

## Updating content later

- **Add a new project card**: duplicate a `.card` block inside `<section id="projects">` in `index.html`.
- **Add a new research entry**: duplicate an `.entry` block inside `<section id="research">`.
- **Swap the CV**: replace `assets/Brayan_Gutierrez_CV.pdf` with an updated file of the same name (or update the link in `index.html` if you rename it).
- **Descriptions to double-check**: the `WaterSafetyClassification` and `STAT_615_Project` / `STAT_553_Project` cards were written from the repo names only (the CV didn't describe them) — edit those blurbs in `index.html` to be accurate.
- No GitHub repository link could be found for the fossil-teeth, EV-OMICS, skeletal-heterochrony, or MD Anderson deconvolution work — if you make those public, add matching cards in the Projects section and `repo-link` lines in Research Experience.

## Local preview

Just open `index.html` in a browser, or run a tiny local server:

```bash
python3 -m http.server 8000
```

then visit `http://localhost:8000`.
