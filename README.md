# Deploying this site (free, via GitHub Pages)

## 1. Create the repository
1. Go to github.com, click **+** → **New repository**.
2. Name it `lloydakresi.github.io` (this exact format gives you the URL `https://lloydakresi.github.io/` with no extra path — recommended). Alternatively, name it anything else (e.g. `personal-site`) and it will be served at `https://lloydakresi.github.io/personal-site/`.
3. Set it to **Public**. Leave it empty (no README, no .gitignore).

## 2. Upload the files
**Option A — web upload (no command line):**
1. Open the new repo, click **Add file → Upload files**.
2. Drag in `index.html`, `styles.css`, and the `assets` folder (with `lloyd-akresi-cv.pdf` and `headshot.jpg` inside).
3. Commit directly to the `main` branch.

**Option B — git:**
```bash
cd path/to/this/folder
git init
git remote add origin https://github.com/lloydakresi/lloydakresi.github.io.git
git add .
git commit -m "Initial site"
git branch -M main
git push -u origin main
```

## 3. Turn on GitHub Pages
1. In the repo, go to **Settings → Pages**.
2. Under "Build and deployment", set **Source** to `Deploy from a branch`.
3. Set **Branch** to `main` and folder to `/ (root)`. Save.
4. Wait 1–2 minutes — your site will be live at the URL GitHub shows there.

## Making future edits
Come back to this conversation (or a new one) and ask Claude to change something — update a project, tweak wording, add a new section. Claude will hand you the updated file(s); re-upload them the same way (Option A overwrites existing files automatically when you drag in files with the same name).

## Files in this folder
- `index.html` — all page content
- `styles.css` — all styling
- `assets/lloyd-akresi-cv.pdf` — downloadable CV
- `assets/headshot.jpg` — profile photo
