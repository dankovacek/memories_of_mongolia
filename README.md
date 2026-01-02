# Memories of Mongolia – Update Guide

Use this guide whenever you need to tweak the public site (hosted by GitHub Pages) without touching anything else in the project.

---

## 1. Local Workflow (beginner-friendly)
These steps assume you have Git installed and are comfortable opening a terminal.

1. **Clone or pull the repository**
   ```bash
   git clone <YOUR_REPO_URL>
   cd memories_of_mongolia
   git pull origin main
   ```
2. **Open the project in a code editor** (VS Code, Sublime, etc.).
3. **Edit the content**
   - Example: to change the title bar text, open `index.html`.
   - Find this line:
     ```html
     <p>Limited digital release</p>
     ```
   - Change it to whatever you want, e.g.:
     ```html
     <p>Now available worldwide</p>
     ```
   - Save the file.
4. **Preview locally (optional but recommended)**
   ```bash
   python -m http.server 8000
   ```
   Visit http://localhost:8000 in your browser and refresh to see the update.
5. **Commit and push**
   ```bash
   git add index.html styles.css
   git commit -m "Update title bar text"
   git push origin main
   ```
6. **Wait for GitHub Pages** – the live site updates automatically within a minute or two after the push. Reload the public URL to confirm.

---

## 2. Windows 11 Workflow (no programming background)
For someone comfortable with tools like Overleaf but not coding, the easiest approach is to edit directly on GitHub.

1. **Sign in to GitHub** in your browser and open the repository page.
2. **Open the file you want to change** (e.g. `index.html`).
3. **Click the pencil icon** at the top-right of the file view to enter edit mode.
4. **Make the change**
   - Example: scroll until you see `<h1>Memories of Mongolia</h1>` and edit the paragraph right below it.
   - Type new text directly in the browser; no extra software is needed.
5. **Scroll to "Commit changes"**
   - Type a short description, e.g. `Update title bar text`.
   - Choose **Commit directly to the main branch**.
   - Click **Commit changes**.
6. **Reload the published site** after about two minutes—GitHub Pages rebuilds automatically when you commit.

> Tip: If you prefer a local copy, download the repository as a ZIP from GitHub ("Code" → "Download ZIP"), unzip it, open `index.html` in Notepad, make changes, and upload the modified file back through GitHub using **Add file → Upload files**. This still avoids any command-line work.

Keep this README handy for future updates so you can quickly refresh the site without needing a developer on hand.
