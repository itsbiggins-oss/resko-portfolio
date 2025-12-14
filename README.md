# RESKO_CMA Portfolio Website

Official portfolio website for **Braylyn "Resko" Stewart** — Louisville graffiti artist and muralist.

🌐 **Live Site:** [reskocma.art](https://reskocma.art)

---

## 📁 Project Structure

```
/
├── index.html          # Main single-page site
├── 404.html            # Custom error page
├── robots.txt          # Search engine crawl rules
├── sitemap.xml         # SEO sitemap
├── og-image.jpg        # Social sharing preview (1200x630px) — YOU CREATE
├── favicon.ico         # Browser tab icon — YOU CREATE
├── favicon-32x32.png   # Favicon 32px — YOU CREATE
├── favicon-16x16.png   # Favicon 16px — YOU CREATE
└── apple-touch-icon.png # iOS home screen icon — YOU CREATE
```

---

## 🚀 Deployment

This is a static site — no build step required. Deploy to any static host:

### Netlify (Recommended)
1. Connect your GitHub repo
2. Set publish directory to `/` (root)
3. Deploy

### GitHub Pages
1. Go to repo Settings → Pages
2. Set source to main branch
3. Custom domain: `reskocma.art`

### Manual Upload
Just upload all files to your web host's public directory.

---

## ⚙️ Configuration

### Update Projects (Archive Section)

Edit the `projects` array in `index.html` (around line 830):

```javascript
const projects = [
    {
        title: "PROJECT NAME",
        category: "museum|justice|collab|mural",  // Filter category
        year: "2024",
        location: "Louisville, KY",
        tags: ["Tag1", "Tag2"],
        desc: "Project description here.",
        color: "border-pink-500",      // Left border accent
        rotate: "1.5deg",              // Card tilt
        tapeRotate: "-2deg"            // Tape strip tilt
    },
    // ... more projects
];
```

**Categories:** `museum`, `justice`, `collab`, `mural`

**Border colors:** `border-pink-500`, `border-cyan-500`, `border-orange-500`, `border-yellow-500`, `border-blue-500`, `border-purple-500`, `border-gray-800`

### Update Commission Form

Replace the Google Form URL in two places in `index.html`:

1. Search for `docs.google.com/forms` 
2. Replace the form ID with your new form's embed URL

### Update Video

Replace the Google Drive video URL in `index.html`:

```html
<iframe src="https://drive.google.com/file/d/YOUR_FILE_ID/preview" ...>
```

**Important:** Ensure the Drive file sharing is set to "Anyone with the link can view"

---

## 🎨 Assets to Create

### Open Graph Image (`og-image.jpg`)
- **Size:** 1200 x 630 pixels
- **Purpose:** Preview image when shared on social media
- **Suggestion:** Hero shot of Resko's work or a branded graphic

### Favicons
Generate all sizes from a single logo using [realfavicongenerator.net](https://realfavicongenerator.net):
- `favicon.ico`
- `favicon-32x32.png`
- `favicon-16x16.png`
- `apple-touch-icon.png` (180x180px)

---

## 🔧 Tech Stack

- **HTML5** — Semantic markup
- **Tailwind CSS** (CDN) — Utility-first styling
- **Chart.js** (CDN) — Data visualizations
- **Google Fonts** — Permanent Marker + Space Grotesk
- **Google Forms** — Commission requests (embedded)
- **Google Drive** — Video hosting

No build tools, no dependencies to install.

---

## 📱 Responsive Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | < 640px | Hamburger nav, stacked layout, simplified effects |
| Tablet | 640-1024px | Hybrid layout |
| Desktop | > 1024px | Full experience with custom cursor, splatters |

---

## 🔍 SEO Checklist

- [x] Meta description
- [x] Open Graph tags
- [x] Twitter Card tags
- [x] Canonical URL
- [x] robots.txt
- [x] sitemap.xml
- [ ] og-image.jpg (create before launch)
- [ ] Favicons (create before launch)
- [ ] Submit sitemap to Google Search Console
- [ ] Submit sitemap to Bing Webmaster Tools

---

## 📝 Content Updates

| To Update | Location | Line # (approx) |
|-----------|----------|-----------------|
| Hero text | `index.html` | ~290 |
| Timeline events | `index.html` | ~370-470 |
| Projects array | `index.html` | ~780-860 |
| Chart data | `index.html` | ~900-970 |
| Contact email | `index.html` | Search "mailto:" |
| Instagram handle | `index.html` | Search "instagram.com" |
| Form URL | `index.html` | Search "docs.google.com/forms" |
| Video URL | `index.html` | Search "drive.google.com" |

---

## 🐛 Known Considerations

- **Google Drive video:** May show Google branding; consider migrating to YouTube/Vimeo for cleaner player
- **Custom cursor:** Disabled on touch devices intentionally
- **Paint splatters:** Disabled on mobile for performance

---

## 📄 License

All content © Braylyn "Resko" Stewart. Website code may be used as reference.

---

## 👤 Contact

- **Artist:** [@resko_cma](https://instagram.com/resko_cma)
- **Site Development:** Christopher @ Fidelity Life

---

*Last updated: December 2024*
