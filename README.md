# 🏛️ IIT Kanpur Course Portal & Semester Planner

A high-performance, mobile-first web application for exploring the IITK course catalog, constructing conflict-free semester schedules, detecting timetable clashes, and calculating academic credit workloads.

Designed with a multi-shade obsidian dark theme, vector typography, and instant client-side filtering across hundreds of courses.

---

## 🚀 Instant 1-Click Deployment

This project is a standalone, dependency-free static web application. It requires zero server setup and can be deployed in seconds to any static hosting provider.

### Option 1: Vercel
1. Push this repository to GitHub / GitLab / Bitbucket.
2. Import the project into [Vercel](https://vercel.com/new).
3. Framework Preset: **Other** (Root directory: `./`).
4. Click **Deploy**. (The included `vercel.json` automatically configures headers and routing).

### Option 2: Netlify
1. Drag and drop the project folder directly into [Netlify Drop](https://app.netlify.com/drop), or connect your Git repository.
2. Publish directory: `.`
3. Click **Deploy**. (The included `netlify.toml` and `_redirects` configure caching, headers, and security rules).

### Option 3: GitHub Pages
1. Push to your GitHub repository.
2. Go to **Settings > Pages**.
3. Under **Branch**, select `main` and root folder `/ (root)`.
4. Click **Save**. Your site will be live at `https://<username>.github.io/<repo-name>/`.

### Option 4: Cloudflare Pages
1. Connect your repository to Cloudflare Pages.
2. Build command: *(leave empty)*
3. Build output directory: `.`
4. Deploy!

---

## 💻 Local Development

Run with Node.js:
```bash
# Clone the repository
git clone <repo-url>
cd "course search"

# Start local server at http://localhost:8888
npm start
```

Or using Python:
```bash
python -m http.server 8888
```

---

## ✨ Features & Architecture

- **⚡ Instant Multi-Token Search**: Search by course code (`CS210`), title (`Data Structures`), instructor (`Sanjay Mittal`), or lecture hall (`L06`, `TB208`). Normalizes hall numbering variants automatically.
- **📅 Interactive Timetable Grid**: Elevated weekly calendar view (Monday–Saturday) with course blocks and instant visual clash alerts.
- **🛡️ Schedule Clash Detector**: Proactively flags time collisions across planned lectures, tutorials, and labs.
- **⭐ Semester Course Planner**: Save courses to calculate total semester credits, weekly contact hours, and export schedules via clipboard.
- **📱 Mobile-First Responsive UX**: Optimized for phones and tablets with slide-up bottom sheets, touch-sized buttons, safe-area inset padding for notched displays, and swipeable timetable scrolling.
- **🎨 Multi-Shade Obsidian Palette**: Handcrafted 6-level grey scale with specular hairline borders, smooth spring transitions, and vector SVG iconography.
- **📱 PWA & Offline Support**: Web App Manifest (`manifest.json`) and Service Worker (`sw.js`) enable offline catalog access and home-screen installation.
- **🖨️ Clean Print Mode**: Dedicated print stylesheet formatted specifically for semester timetable exports.

---

## 📁 Repository Structure

```
├── index.html          # Core single-page application (HTML, CSS, JS engine)
├── Course Schedule...  # Primary IITK course CSV dataset
├── manifest.json       # Progressive Web App manifest
├── sw.js               # Service worker for offline caching
├── favicon.svg         # High-resolution vector favicon
├── icon-192.png        # PWA app icon (192x192)
├── icon-512.png        # PWA app icon (512x512)
├── netlify.toml        # Netlify production configuration & cache policies
├── vercel.json         # Vercel deployment configuration & security headers
├── _redirects          # SPA fallback routing for static hosts
├── robots.txt          # Search engine crawler instructions
├── package.json        # Node development scripts
└── README.md           # Documentation & deployment guide
```

---

## 📜 License
MIT License. Created for the IIT Kanpur student community.
