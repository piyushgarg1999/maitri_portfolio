# Maitree Jain – Portfolio Website

A professional, recruiter-friendly portfolio for **MBA in Digital Transformation**, built with HTML, CSS, and JavaScript. Suitable for consulting, product, digital strategy, and analytics roles.

---

## Deploy on GitHub (quick steps)

The project is already a git repo with one commit. To put it on GitHub and go live:

1. **Create a new repo on GitHub**
   - Go to [github.com/new](https://github.com/new).
   - Repository name: `Maitri_Portfolio` (or any name you like).
   - Choose **Public**. Do **not** add a README, .gitignore, or license (you already have files).
   - Click **Create repository**.

2. **Push your code** (replace `YOUR_USERNAME` with your GitHub username):
   ```bash
   cd /Users/Piyush_Garg/Maitri_Portfolio
   git remote add origin https://github.com/YOUR_USERNAME/Maitri_Portfolio.git
   git branch -M main
   git push -u origin main
   ```

3. **Turn on GitHub Pages**
   - In the repo, go to **Settings** → **Pages** (left sidebar).
   - Under **Source**, choose **Deploy from a branch**.
   - Branch: **main**, Folder: **/ (root)**.
   - Click **Save**.

4. **Your site will be live in 1–2 minutes at:**
   - `https://YOUR_USERNAME.github.io/Maitri_Portfolio/`

---

## Project structure

```
Maitri_Portfolio/
├── index.html          # Main page (all sections)
├── css/
│   └── styles.css     # All styles
├── js/
│   └── main.js        # Nav toggle, smooth scroll, footer year
├── Maitree_Jain_CV.pdf # Resume (download link)
└── README.md          # This file
```

## How to update content

### 1. Personal & contact info
- **Name / title / tagline:** In `index.html`, edit the **Hero** section (`#hero`): `.hero-title`, `.hero-subtitle`, `.hero-tagline`.
- **Email / LinkedIn:** In the **Contact** section (`#contact`), update the `href` and link text for the email and LinkedIn links.
- **Resume file:** Keep `Maitree_Jain_CV.pdf` in the project root and the link will work. To use another file, replace the PDF and change the link in both the hero “Download Resume” button and the contact “Download Resume” link.

### 2. About Me
- In `index.html`, find the section `id="about"` and edit the paragraphs inside `.about-content`.

### 3. Skills
- In `index.html`, find `id="skills"` and the `.skills-grid`. Each skill is a `.skill-card` with an `h3` (title) and `p` (description). Add, remove, or edit cards to match your resume.

### 4. Projects / case studies
- In `index.html`, find `id="projects"` and the `.projects-list`. Each project is an `<article class="project-card">` with:
  - `h3` – project title  
  - `p.project-meta` – domain/tags (e.g. Strategy · Data)  
  - `p` – short description  
Copy from your resume or add new cards. You can remove the “Update the above…” note when done.

### 5. Experience / internships
- In `index.html`, find `id="experience"` and the `.timeline`. Each role is a `.timeline-item` with:
  - `h3` – role and company  
  - `p.timeline-meta` – duration and location  
  - `p` – description  
Duplicate a `.timeline-item` block to add more roles. Remove the “Copy your experience…” note when done.

### 6. Education & certifications
- In `index.html`, find `id="education"` and the `.education-list`. Each item is an `.edu-card` with degree/cert name, `.edu-meta` (institution, year), and a paragraph. Add or edit cards and remove the “Fill in your actual…” note when done.

### 7. Page title and SEO
- In `index.html`, inside `<head>`:
  - `<title>` – browser tab title.
  - `<meta name="description">` – short summary for search results.
  - `<meta name="keywords">` – optional keywords.
  - `<meta property="og:...">` – optional; used when the link is shared on social.

After editing, commit and push; your host (GitHub Pages / Netlify / Vercel) will update the live site.

---

## Deployment (free hosting)

### Option A: GitHub Pages

1. **Create a GitHub repo**
   - Go to [github.com/new](https://github.com/new).
   - Name it `Maitri_Portfolio` (or any name; the site will be `https://<username>.github.io/<repo-name>/`).
   - Public, no need to add README if the folder is already a git repo.

2. **Push your project**
   ```bash
   cd /Users/Piyush_Garg/Maitri_Portfolio
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/Maitri_Portfolio.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Repo → **Settings** → **Pages**.
   - Under **Source**, choose **Deploy from a branch**.
   - Branch: **main**, folder: **/ (root)**.
   - Save. In a few minutes the site will be at `https://YOUR_USERNAME.github.io/Maitri_Portfolio/`.

### Option B: Netlify

1. Go to [netlify.com](https://www.netlify.com) and sign up / log in.
2. **Add new site** → **Import an existing project** → **Git**.
3. Connect GitHub and select the repo (or upload the folder with **Deploy manually**).
4. Build settings:
   - **Build command:** leave empty.
   - **Publish directory:** `/` or `.`
5. Deploy. Netlify will give you a URL like `https://random-name.netlify.app`. You can set a custom name in **Domain settings**.

### Option C: Vercel

1. Go to [vercel.com](https://vercel.com) and sign up / log in (e.g. with GitHub).
2. **Add New** → **Project** → import the repo.
3. **Root Directory:** leave as `.`
4. **Framework Preset:** Other (no framework).
5. Deploy. You’ll get a URL like `https://maitri-portfolio-xxx.vercel.app`. You can add a custom domain in project settings.

---

## Tech stack

- **HTML5** – semantic sections, accessibility-friendly.
- **CSS3** – variables, Grid, Flexbox, responsive layout.
- **JavaScript** – minimal (mobile menu, smooth scroll, current year).
- **Fonts:** DM Sans (UI), Instrument Serif (headings), from Google Fonts.

No build step or backend; static files only.

---

## SEO

- Meta description and keywords in `<head>`.
- Open Graph tags for link previews.
- Semantic headings (one `h1`, then `h2`/`h3`).
- Descriptive section IDs for anchor links.

---

## License

Content and design are yours. Use and modify as you like.
