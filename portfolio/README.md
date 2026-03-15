# Rishabh Bahuguna · Portfolio

Personal portfolio website for Product Analyst / APM job search.

## Folder structure

```
rishabhbahuguna03.github.io/
├── index.html              ← main page (edit content here)
├── assets/
│   ├── css/
│   │   └── style.css       ← all visual styles (edit design here)
│   ├── js/
│   │   └── main.js         ← interactions & animations
│   └── images/             ← put project screenshots here
└── README.md
```

## How to deploy to GitHub Pages

### Option A — Upload via GitHub website (easiest, no Git required)

1. Go to https://github.com/Rishabhbahuguna03/rishabhbahuguna03.github.io
2. Click **Add file → Upload files**
3. Drag and drop all three files/folders:
   - `index.html`
   - `assets/` folder (with css and js inside)
4. Scroll down → click **Commit changes**
5. Your site updates at https://rishabhbahuguna03.github.io within ~60 seconds

### Option B — VSCode + Git (recommended for ongoing edits)

```bash
# 1. Clone your repo
git clone https://github.com/Rishabhbahuguna03/rishabhbahuguna03.github.io.git
cd rishabhbahuguna03.github.io

# 2. Replace files with the new ones from this zip
#    (copy index.html and assets/ folder into the repo folder)

# 3. Push to GitHub
git add .
git commit -m "Revamp portfolio — new structure, about section, rewritten projects"
git push origin main
```

Your site is live at https://rishabhbahuguna03.github.io

---

## How to edit content

All `EDIT:` comments in `index.html` mark exactly what to change.

| What to change | Where |
|---|---|
| Hero tagline / name | `index.html` → hero section |
| About paragraphs | `index.html` → about section |
| Add a new project | Copy a `project-card` block in the projects section |
| Skills list | `index.html` → skills section |
| Social links / email | Contact section + nav `href` values |
| Colours | `style.css` → `:root` variables at top |
| Fonts | `style.css` → `:root` + Google Fonts link in `<head>` |

## How to add a new project

1. Open `index.html`
2. Find the `projects-grid` div
3. Copy this block and paste it **above** the existing cards:

```html
<div class="project-card featured reveal">
  <div class="project-img">
    <div class="project-img-inner">📊</div>
  </div>
  <div class="project-body">
    <div class="project-meta">
      <span class="project-type">Your category</span>
    </div>
    <h3 class="project-title">Your project title</h3>
    <p class="project-desc">Problem → what you did → how you did it.</p>
    <p class="project-insight">Key finding with a number attached.</p>
    <div class="project-tools">
      <span class="tool-tag">SQL</span>
      <span class="tool-tag">Python</span>
    </div>
    <a class="project-link" href="YOUR_GITHUB_LINK" target="_blank">View on GitHub</a>
  </div>
</div>
```

4. Remove `class="featured"` from the old top card
5. Save → push to GitHub

## Colour customisation

Edit the CSS variables at the top of `style.css`:

```css
:root {
  --ink:     #1a1a18;   /* main text colour */
  --accent:  #c84b2f;   /* red-orange highlights */
  --accent2: #1d5c8a;   /* blue links and badges */
  --paper:   #f7f5f0;   /* page background (warm white) */
}
```
