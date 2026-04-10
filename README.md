# Felipe Villasuso Lago – Personal Academic Website

A static, professional personal website for **Felipe Villasuso Lago**, PhD researcher at London South Bank University, corporate lawyer, and governance scholar. Built with plain HTML and CSS — no frameworks, no build tools required — and designed to be deployed via **GitHub Pages**.

---

## Live Site

Once deployed, the site will be accessible at:

```
https://felipelago17.github.io/Background-and-Publications/
```

---

## Site Structure

```
/
├── index.html          # Home page (biography overview, key areas, recent publications)
├── about.html          # Detailed biography, education, and areas of expertise
├── experience.html     # Professional career history and core competencies
├── publications.html   # Full publication list organised by category
├── research.html       # Research themes, PhD project, and collaboration opportunities
├── contact.html        # Contact information and academic profiles
├── css/
│   └── style.css       # Shared stylesheet (responsive, academic design)
└── README.md           # This file
```

---

## Deploying via GitHub Pages

### Option A – Deploy from the `main` branch (recommended)

1. Push all files to the `main` branch of this repository.
2. In the repository on GitHub, go to **Settings → Pages**.
3. Under **Source**, select **Deploy from a branch**.
4. Choose **Branch: `main`** and **Folder: `/ (root)`**.
5. Click **Save**.
6. After a few minutes, the site will be live at `https://felipelago17.github.io/Background-and-Publications/`.

### Option B – Deploy from a `gh-pages` branch

1. Create a branch named `gh-pages` and push the website files to it.
2. Go to **Settings → Pages → Source**.
3. Select **Branch: `gh-pages`** and **Folder: `/ (root)`**, then click **Save**.

### Option C – Deploy from a `/docs` folder

1. Move all HTML/CSS files into a folder named `docs/` at the repository root.
2. Go to **Settings → Pages → Source**.
3. Select **Branch: `main`** and **Folder: `/docs`**, then click **Save**.

---

## Keeping the Site Up to Date

### Adding a new publication

Open `publications.html` and add a new `<article class="pub-item">` block inside the appropriate section:

```html
<article class="pub-item">
  <span class="card-tag tag-conf">Conference Paper</span>
  <h3>"Your Title Here"</h3>
  <p class="authors"><strong>Villasuso Lago, F.</strong>, Co-Author, A.</p>
  <p class="venue">
    <em>Journal / Conference Name</em>, Year. DOI: ...
  </p>
  <p>Short abstract or description.</p>
  <p class="doi-link">
    <a href="https://doi.org/..." target="_blank" rel="noopener">DOI Link ↗</a>
  </p>
</article>
```

Publication type tags available:
- `tag-book` – Book chapters
- `tag-conf` – Conference papers
- `tag-article` – Policy articles / journal articles
- `tag-report` – Working papers / reports

### Adding a new experience entry

Open `experience.html` and add a `<div class="timeline-item">` block inside the `.timeline` container:

```html
<div class="timeline-item">
  <p class="timeline-date">2025 – Present</p>
  <h3 class="timeline-title">New Role Title</h3>
  <p class="timeline-org">Organisation Name, Location</p>
  <p>Brief description of responsibilities and achievements.</p>
</div>
```

---

## Design Notes

- **No dependencies** – pure HTML5 and CSS3; no JavaScript libraries required.
- **Responsive** – adapts to mobile, tablet, and desktop screen sizes.
- **Accessible** – semantic HTML, skip-to-content link, ARIA labels, keyboard-navigable.
- **SEO-friendly** – `<meta>` description/keywords, Open Graph tags, and JSON-LD structured data on the home page.
- **Academic tone** – professional colour palette (deep navy and gold), clean typography.

---

## Local Preview

Because the site uses only static files with relative paths, you can preview it locally in two ways:

**Method 1 – Open directly in a browser:**
```
# On macOS
open index.html

# On Linux
xdg-open index.html

# On Windows
start index.html
```

**Method 2 – Use Python's built-in server (recommended for accurate link resolution):**
```bash
python3 -m http.server 8000
# Then open http://localhost:8000 in your browser
```

---

## Contact

For questions about the content of this website, please contact Felipe via:

- **LinkedIn:** https://www.linkedin.com/in/felipe-villasuso-lago-54047a122/
- **ORCID:** https://orcid.org/0009-0002-0542-3216
- **Academia.edu:** https://lsbu.academia.edu/FelipeLago
- **ResearchGate:** https://www.researchgate.net/profile/Felipe-Villasuso-Lago
