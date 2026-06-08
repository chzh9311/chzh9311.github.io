# Personal Academic Website

A clean, fast Jekyll site. Cream + gold + teal palette, Stencil-inspired typography, two-column homepage layout.

---

## Quick Start: Run Locally

### Prerequisites

Install Ruby (via rbenv or system package manager):

```bash
# macOS (Homebrew)
brew install ruby rbenv
rbenv install 3.2.0 && rbenv global 3.2.0

# Ubuntu/Debian
sudo apt install ruby-full build-essential zlib1g-dev
```

### Install & Serve

```bash
# 1. Clone or enter the project folder
cd personal-site

# 2. Install Jekyll + dependencies
gem install bundler
bundle install

# 3. Serve locally with live reload
bundle exec jekyll serve --livereload

# → Open http://localhost:4000
```

Any file change auto-rebuilds and reloads the browser.

---

## Deploy to GitHub Pages (automatic, free)

### One-time setup

1. **Create a GitHub repo** named `your-username.github.io`
   (or any name if you want a project page at `your-username.github.io/repo-name`)

2. **Push this folder** to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages** in the repo:
   - Go to **Settings → Pages**
   - Under *Source*, select **GitHub Actions**
   - Save

4. GitHub automatically runs `.github/workflows/deploy.yml` on every push.
   Your site will be live at `https://your-username.github.io` in ~1 minute.

### Subsequent updates

```bash
# Edit any file, then:
git add .
git commit -m "Update bio / add paper / ..."
git push
# → Site redeploys automatically in ~60 seconds
```

---

## How to Maintain the Site

### Change your personal info
Edit `_config.yml` — name, email, GitHub, Google Scholar ID, affiliation.

### Add a news item
Open `_data/news.yml` and prepend a new entry:
```yaml
- date: "Jan. 2027"
  text: "One paper accepted by "
  link: "https://neurips.cc"
  link_text: "NeurIPS'27"
```

### Add a publication
Open `_data/publications.yml` and prepend:
```yaml
- title: "Your Paper Title"
  authors: "{self}Your Name, Coauthor One, Supervisor*"
  venue: "Conference/Journal Name, Year"
  pdf: "https://arxiv.org/abs/XXXX.XXXXX"
  code: "https://github.com/you/project"
  page: ""   # optional project page
```
Use `{self}` immediately before your name — it bolds it automatically.

### Replace your photo
Drop a square image at `assets/img/avatar.jpg` (or `.png`) and update `_config.yml`:
```yaml
avatar: /assets/img/avatar.jpg
```

### Add your CV
Drop a PDF at `assets/cv.pdf` and update `_config.yml`:
```yaml
cv_url: /assets/cv.pdf
```

### Adjust colours or fonts
All tokens are in `assets/css/main.scss` at the top under `:root { ... }`.

---

## File Structure

```
personal-site/
├── _config.yml          ← site-wide settings (name, email, links)
├── _data/
│   ├── news.yml         ← news entries
│   └── publications.yml ← paper list
├── _layouts/
│   └── default.html     ← HTML shell (nav + footer)
├── _includes/
│   └── profile.html     ← left sidebar (photo + links)
├── _pages/
│   └── publications.html← /publications/ page
├── assets/
│   ├── css/main.scss    ← all styles + design tokens
│   └── img/avatar.jpg   ← your photo (add this)
├── index.html           ← homepage
├── Gemfile              ← Ruby dependencies
└── .github/workflows/
    └── deploy.yml       ← auto-deploy to GitHub Pages
```
