# Dr. Hamdy Soliman — Academic Website

A fully self-contained static website. No local server needed — works directly on GitHub Pages.

---

## File Structure

```
your-repo/
├── index.html              ← Home page
├── publications.html       ← Publications (loads XML dynamically)
├── research.html           ← Research interests & labs
├── courses.html            ← Courses taught
├── shared.css              ← All custom styles
└── xml/
    ├── publication_journal.xml
    ├── publication_conference.xml
    ├── publication_books.xml
    └── publication_grants.xml
```

> **Note:** The `research.html` page references images from a `doc_images/` folder (e.g. `doc_images/sensor_1.png`). Add that folder to your repo if you have those images. Otherwise the page shows a placeholder.

---

## Deploy to GitHub Pages (free, ~5 minutes)

### Step 1 — Create a GitHub account
Go to https://github.com and sign up if you don't have an account.

### Step 2 — Create a new repository
1. Click the **+** button → **New repository**
2. Name it: `hamdy-soliman` (or anything you like)
3. Set it to **Public**
4. Click **Create repository**

### Step 3 — Upload your files
1. On your new repo page, click **uploading an existing file**
2. Drag and drop ALL files and folders:
   - `index.html`
   - `publications.html`
   - `research.html`
   - `courses.html`
   - `shared.css`
   - The entire `xml/` folder (drag the folder itself)
3. Scroll down, click **Commit changes**

### Step 4 — Enable GitHub Pages
1. Go to your repo → **Settings** tab
2. In the left sidebar click **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Set Branch to **main** and folder to **/ (root)**
5. Click **Save**

### Step 5 — Your site is live!
Within 1–2 minutes your site will be at:
```
https://YOUR-USERNAME.github.io/hamdy-soliman/
```
GitHub will show the exact URL in the Pages settings.

---

## Updating publications
Just edit the XML files in the `xml/` folder and re-upload them to GitHub. The HTML pages fetch them automatically — no code changes needed.

## Adding photos (optional)
Create a `doc_images/` folder in your repo and upload images named:
- `sensor_1.png`, `security_2.png` — Research lab photos (research.html)
- `nmt_logo.png` — NMT logo for footer
- `field_1_1.png` through `field_1_4.png` — Field research carousel

---

## Alternative free hosting options

| Platform | URL | Setup difficulty |
|----------|-----|-----------------|
| **GitHub Pages** ✅ | `username.github.io/repo` | Easy, recommended |
| **Netlify** | `yoursite.netlify.app` | Very easy — drag & drop folder |
| **Vercel** | `yoursite.vercel.app` | Easy — connect GitHub repo |

**Netlify** is the fastest if you just want to drag-and-drop a folder with zero Git knowledge:
1. Go to https://netlify.com → Sign up
2. Drag your entire site folder onto the Netlify dashboard
3. Done — you get a live URL instantly
