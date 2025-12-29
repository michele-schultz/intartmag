# International Art Magazine (I.A.M.) - Project Summary

> A modern, vanilla web application showcasing contemporary art news, reviews, and cultural discourse focused on international art with emphasis on the New York art scene.

**Repository:** [github.com/adamaslan/intartmag](https://github.com/adamaslan/intartmag)

---

## Tech Stack

| Category | Technology |
|----------|------------|
| **Frontend** | HTML5, CSS3, Vanilla JavaScript |
| **CSS Framework** | Bootstrap 4.0.0 (CDN) |
| **JavaScript Libraries** | jQuery 3.2.1 (slim), Popper.js 1.12.9 |
| **Analytics** | Google Analytics (UA-91787385-1) |
| **Newsletter** | ConvertKit integration |
| **Image CDN** | Cloudinary (partial) |
| **Server** | Apache (.htaccess URL rewriting) |

---

## Directory Structure

```
intartmag/
├── index.html              # Main landing page
├── pages/                  # 56 article pages
│   ├── galleries.html
│   ├── culture.html
│   └── [50+ article pages]
├── images/                 # 125 media files (153MB)
├── style/                  # CSS stylesheets
│   ├── style.css           # Main stylesheet (194 lines)
│   ├── dog.css             # Alternate styling
│   └── dog*.css            # Style variants
├── fonts/                  # Custom fonts (opera, plantin, teletype, utopia)
├── includes/
│   └── navbar.html         # Reusable navigation component
├── newsletter-popup.js     # Newsletter modal (ConvertKit)
├── parallax.js             # Scroll effects
└── .htaccess               # URL rewriting rules
```

---

## Key Features

### 1. Magazine Platform
- 56 article pages covering art exhibitions, galleries, and cultural events
- Featured articles with preview text on homepage
- Categories: Home, Galleries, Culture

### 2. Responsive Navigation
- Fixed top navbar with hamburger menu (mobile)
- Scroll-triggered color transitions (transparent → pink/green)
- Bootstrap 4 collapse functionality

### 3. Newsletter Subscription
- Modal popup (3-second delay after page load)
- ConvertKit form integration
- Email + first name collection

### 4. Visual Effects
- Parallax scrolling backgrounds
- Navbar scroll animations
- Responsive image layouts with figure/figcaption

---

## Typography

| Element | Font Family |
|---------|-------------|
| Body | Space Grotesk (sans-serif) |
| Headings | Spectral (serif) |
| Navbar/Decorative | Rakkas (cursive) |
| Display | Playfair Display |
| Sans | Karla |

---

## Content Categories

- **Gallery Reviews** - Barbara Ess, Diana NY, Magenta Plains, etc.
- **Artist Profiles** - Interviews and features
- **Art Events** - Art Basel, Armory Show, Art Week LA
- **Cultural Pieces** - Museums, installations, art discourse
- **International Art** - Istanbul, European galleries
- **Lifestyle** - Wine, spirits, food culture
- **NYC Focus** - Bushwick, Tribeca, Chinatown, LIC galleries

---

## Responsive Breakpoints

| Width | Device |
|-------|--------|
| 1024px | Tablet |
| 768px | Mobile Landscape |
| 600px | Mobile |
| 480px | Small Mobile |

---

## Color Scheme

- **Primary Red:** `#c1121f`
- **Background:** White
- **Text:** Black
- **Navbar (scrolled):** Pink/Green variants

---

## Files Overview

| File | Purpose | Size |
|------|---------|------|
| `index.html` | Main landing page | 65KB |
| `style/style.css` | Primary stylesheet | 8KB |
| `newsletter-popup.js` | Newsletter modal | 4KB |
| `parallax.js` | Scroll effects | 1KB |
| `includes/navbar.html` | Reusable nav | 1KB |
| `images/` | Media assets | 153MB |

---

## Known Issues

1. **Typography Bug** - `.body` selector instead of `body` prevents base font from applying
2. **Layout** - Fixed 70% width without max-width causes long lines on large screens
3. **Accessibility** - Missing alt attributes on some images
4. **Performance** - Multiple Google Font families increase page weight
5. **Images** - Missing srcset/lazy-loading for optimization

---

## Development

**Current Branch:** `trib6`
**Main Branch:** `main`

### Recent Commits
```
2a575fc links-text2
6f77d2c links-text
65a8245 trib4bc
00278de trib4b
35d5582 trib4
```

---

## Deployment

- **Type:** Static HTML site (no build process)
- **Server:** Apache with .htaccess URL rewriting
- **Hosting:** FTP-based deployment
- **URLs:** Clean URLs without .html extension

---

## Quick Start

1. Clone the repository
2. Serve files with any static server (Apache recommended for .htaccess support)
3. Open `index.html` in browser

For local development without Apache:
```bash
# Python 3
python -m http.server 8000

# Node.js
npx serve
```

---

## Project Stats

- **Total Articles:** 56 pages
- **Image Assets:** 125 files
- **Total Size:** ~301MB
- **CSS Files:** 4
- **JavaScript Files:** 2