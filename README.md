
# ITC Website — Institute Technical Council, IIT Bombay

A multi-page, fully responsive website for the **Institute Technical Council (ITC), IIT Bombay**, built as Task 1 of the ITC Web Convener Application 2026.

---

## 📁 Project Structure

```
ITC website/
├── index.html          # Home page
├── about.html          # About page
├── events.html         # Events page
├── team.html           # Meet the Team page
├── contact.html        # Contact page
├── style.css           # Global styles — dark theme, CSS variables, animations
├── main.js             # Shared JS — scroll animations, mobile menu, active nav
├── icons/
│   ├── build.svg
│   ├── calendar.svg
│   ├── check.svg
│   ├── facebook.svg
│   ├── idea.svg
│   ├── instagram.svg
│   ├── location.svg
│   ├── mail.svg
│   ├── map.svg
│   ├── people.svg
│   ├── phone.svg
│   └── twitter.svg
└── images/
    └── teams/
        ├── core_team2022.png
        ├── pg_team_poster.png
        ├── team-media.png
        ├── team_design.png
        └── team_web.png
```

---

## 📄 Pages

| Page | File | Description |
|---|---|---|
| Home | `index.html` | Hero section, stats, scrolling clubs strip, about snapshot, events teaser, CTA |
| About | `about.html` | Mission, org structure timeline, how to join, clubs showcase |
| Events | `events.html` | Filterable event cards — All / Upcoming / Past / Annual |
| Meet the Team | `team.html` | ITC cabinet, club conveners & managers, web/creatives/PG teams |
| Contact | `contact.html` | Contact form with validation, social links, address, map |

---

## ✨ Features

- Fully responsive — works on desktop, tablet, and mobile
- Dark theme with blue/violet gradient accent palette
- Sticky navbar with scroll effect and active page highlight
- Mobile hamburger menu with animated open/close
- Scroll-triggered fade-up animations using IntersectionObserver
- Auto-scrolling clubs strip on the home page
- Event filter tabs — filter by type without page reload
- Contact form with client-side validation and success state
- Smooth page fade-in on load
- Real ITC data — content pulled from itc.gymkhana.iitb.ac.in

---

## 🛠️ Tech Stack

- **HTML5** — semantic structure across all 5 pages
- **CSS3** — custom properties, flexbox, grid, keyframe animations
- **Vanilla JavaScript** — no frameworks, no dependencies
- **Google Fonts** — Syne (headings) + DM Sans (body)

---

## 🎨 Design System

All design tokens are defined as CSS variables in `style.css`:

```css
--bg:            #080b12      /* page background */
--bg-card:       #0d1120      /* card background */
--accent-blue:   #3b82f6      /* primary accent */
--accent-violet: #7c3aed      /* secondary accent */
--accent-grad:   linear-gradient(135deg, #3b82f6, #7c3aed)
--text-primary:  #f0f4ff
--text-secondary:#8b95b0
--text-muted:    #4a5270
```

---

## 🚀 Running Locally

No build step needed — just open the HTML files directly.

**Option 1 — Open in browser:**
```
Double-click index.html
```

**Option 2 — Use VS Code Live Server:**
1. Install the Live Server extension in VS Code
2. Right-click `index.html` → **Open with Live Server**

---

## 🌐 Deployment

Deployed on Vercel. To deploy yourself:

1. Push the `ITC website/` folder to a GitHub repository
2. Go to [vercel.com](https://vercel.com) → New Project → Import repo
3. Set:
   ```
   Framework:     Other
   Root Directory: ITC website
   ```
4. Click Deploy

---

## 📋 File Responsibilities

**`style.css`**
- CSS variables for the entire design system
- Navbar, footer, card, button, badge, form styles
- Page hero shared styles
- Scroll animation classes (`.animate`, `.visible`)
- Responsive breakpoints for mobile and tablet

**`main.js`**
- Navbar background change on scroll
- Hamburger menu toggle with X animation
- `IntersectionObserver` for staggered scroll animations
- Active nav link detection based on current page filename
- Page fade-in on load

---

## 👤 Author

**Sarbjeet Singh Pal**
B.Tech Economics, IIT Bombay
ITC Web Convener Application — April 2026
