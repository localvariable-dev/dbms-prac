# VS Code–Inspired AI Lab Practicals

A single-page, interactive learning workspace styled after Visual Studio Code's familiar Dark+ theme. The polish pass keeps the original palette and UI concept while refining spacing, interaction feedback, scrollbars, and smaller-screen layout.

## Project structure

```text
dbms-vscode-practicals/
├── index.html          # Complete standalone site (HTML, CSS, and JavaScript)
├── README.md           # Project and GitHub Pages instructions
├── .nojekyll           # Prevents GitHub Pages from running Jekyll
└── assets/
    └── .gitkeep       # Reserved for future local assets
```

There are no build steps or dependencies. All site code is currently contained in `index.html`.

## Preview locally

Open `index.html` in a modern browser. For a local server, from this folder run:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Publish with GitHub Pages

1. Create a **Public** GitHub repository (for example, `dbms-vscode-practicals`).
2. In Terminal, from this project folder, run:

   ```bash
   git init
   git add .
   git commit -m "Polish VS Code-inspired practicals workspace"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/dbms-vscode-practicals.git
   git push -u origin main
   ```

3. On GitHub, open **Settings → Pages**.
4. Set **Source** to `Deploy from a branch`, branch to `main`, and folder to `/ (root)`, then Save.
5. After the Pages deployment finishes, the site will be available at:

   `https://YOUR_USERNAME.github.io/dbms-vscode-practicals/`

Replace `YOUR_USERNAME` with your GitHub username.

## Updating the deployed site

After editing files locally:

```bash
git add .
git commit -m "Update website"
git push
```

GitHub Pages will redeploy the pushed changes.
