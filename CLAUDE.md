# ITC Project — IITB Tech Council Website

## Overview
Static website for the IIT Bombay Tech Council. Deployed on Vercel.

## Project Structure
- `ITC website/` — Main site served by Vercel (HTML, CSS, JS)
  - `index.html` — Homepage
  - `about.html`, `contact.html`, `events.html`, `team.html` — Subpages
  - `style.css` — Styles
  - `main.js` — Client-side JS
  - `images/`, `icons/` — Assets
  - `design/` — Design system assets
- `*_files/` directories — Supporting assets copied into `ITC website/` at build time
- `vercel.json` — Vercel deployment config (build copies `*_files` dirs, output = `ITC website/`)
- `design-system/` — Design reference (`itc-bombay`)

## Build & Deploy
- **Platform:** Vercel
- **Build command:** `for d in *_files; do cp -r "$d" "ITC website/"; done`
- **Output directory:** `ITC website`
- No build tool / bundler — plain static files

## Development
- Open any HTML file in a browser to preview locally
- No dev server required

## Conventions
- Plain HTML/CSS/JS — no framework
- Keep file and folder names as-is (spaces in paths are intentional)
