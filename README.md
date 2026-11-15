# Academic website (Quarto + GitHub Pages)

## 1. Personalize
- The whole site is one page: edit `index.qmd` (about, research, teaching, references) and the links/name in `_quarto.yml`.
- Replace `images/profile.jpg` with your headshot (portrait orientation works best; it is shown in black and white and turns to colour on hover).
- Colours and fonts are set at the top of `styles.scss`.
- Put PDFs in `files/`: `cv.pdf`, `jmp.pdf`, etc.

## 2. Preview locally
Install Quarto from https://quarto.org/docs/get-started/ then run:

    quarto preview

## 3. Publish on GitHub
1. Create a public repo named **`YOUR-USERNAME.github.io`** (gives you the URL `https://YOUR-USERNAME.github.io`).
2. Push this folder:

       git init
       git add .
       git commit -m "Initial site"
       git branch -M main
       git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git
       git push -u origin main

3. On GitHub: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
4. Every push to `main` rebuilds the site (see the **Actions** tab). Live in ~1–2 minutes.

## Updating
Edit a `.qmd` file or replace a PDF in `files/`, then commit and push.
