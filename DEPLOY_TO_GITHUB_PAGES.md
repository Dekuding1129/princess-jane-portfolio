# Deploy to GitHub Pages

This folder is already prepared as a Git repository for GitHub Pages.

## Files

- `index.html` — the page GitHub Pages will serve
- `princess-jane-profile.png` — profile image
- `PRINCESS TTL2.pptx` — downloadable PowerPoint
- `Class_Record_EXCEL.xlsx` — downloadable Excel project
- `.nojekyll` — tells GitHub Pages to serve the files as plain static files

## 1. Create the GitHub repository

1. Go to https://github.com/new
2. Repository name example:

```text
princess-jane-portfolio
```

3. Set it to `Public`.
4. Do not add README, .gitignore, or license from GitHub because this folder already has files.
5. Click `Create repository`.

## 2. Connect this local folder to GitHub

Replace `YOUR_USERNAME` with your GitHub username:

```bash
cd "/mnt/c/Users/Acer PC/Desktop/html crash cource/.vscode/Princess"
git remote add origin https://github.com/YOUR_USERNAME/princess-jane-portfolio.git
git push -u origin main
```

If Git asks for login:

```text
Username: your GitHub username
Password: paste a GitHub Personal Access Token, not your GitHub password
```

Personal Access Token page:

```text
https://github.com/settings/tokens
```

For a classic token, select at least:

```text
repo
workflow
```

## 3. Enable GitHub Pages

In the GitHub repository:

```text
Settings → Pages
```

Set:

```text
Source: Deploy from a branch
Branch: main
Folder: /root
```

Click `Save`.

## 4. Open the website

After 1–3 minutes, GitHub Pages will show the public link. It usually looks like:

```text
https://YOUR_USERNAME.github.io/princess-jane-portfolio/
```

## 5. If you edit the site later

Run:

```bash
cd "/mnt/c/Users/Acer PC/Desktop/html crash cource/.vscode/Princess"
git add .
git commit -m "Update portfolio site"
git push
```
