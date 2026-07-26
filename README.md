# Nilabh Pandey — Portfolio

Personal portfolio website showcasing AI research, robotics projects, IEEE publications, and professional experience — designed as a "mission control" interface inspired by the drone imaging and object-detection work it presents.

**Live:** [https://nilabhpandy.com](https://nilabhpandy.com)

## Features

- **Multi-language support** — English, German, French, Portuguese, Spanish, and Hindi with instant switching, translated page titles, and persistent selection (works on mobile too)
- **Dark / Light mode** — Dark by default, toggle saved across sessions, with a theme-aware starfield and browser theme-color
- **Detection-frame hero** — The name renders inside an animated YOLO-style bounding box with corner brackets and a confidence label, plus a decode/scramble intro and a typewriter role rotator
- **Starfield background** — Orange & purple constellation with connecting lines, mouse parallax, twinkling, and occasional shooting stars (pauses when the tab is hidden)
- **Scanning portrait** — Photo framed by target brackets with a sensor sweep and a telemetry readout strip
- **Boot sequence** — A quick mission-control "systems online" intro, shown once per session
- **Filterable projects** — One-tap filters (AI & ML / Robotics & Drones / IoT & Embedded / Blockchain) with animated re-flow and sequential numbering that renumbers as you filter
- **Live telemetry** — The hero readout includes a real-time Zurich clock alongside coordinates and system status
- **Copy email** — One-click copy button on the contact card with a translated confirmation toast
- **Micro-interactions** — Cursor-tracking spotlight on every card, subtle 3D tilt, magnetic buttons, count-up hero stats, skill-count badges, animated tech ticker, shimmering gradient text, hero parallax on scroll, scroll progress bar, staggered blur-reveal, and click the hero name to re-run the decode effect
- **Custom cursor** — Dot + glow ring, enabled only on precise pointers (mouse/trackpad), so touch devices are unaffected
- **Fully responsive** — Dedicated mobile menu with staggered links; language and theme controls stay visible on small screens
- **Accessible & robust** — Respects `prefers-reduced-motion`, visible keyboard focus, skip-to-content link, ARIA labels, safe `localStorage` (no crash in private browsing), and a graceful placeholder if the profile photo is missing
- **SEO ready** — Open Graph / Twitter cards, canonical URL, JSON-LD person schema, and a meta description that switches language with the site
- **Print-friendly** — A dedicated print stylesheet turns the page into a clean, resume-style document
- **Works without JavaScript** — Full content remains readable thanks to a noscript fallback

## Sections

Hero · About · Experience · Education · Publications · Projects · Skills & Tools · Certifications · Contact

## Setup

1. Create a GitHub repository named `<your-username>.github.io`
2. Upload `index.html` and `Nilabh_Pandey_Image.jpg` to the root of the repository
3. Go to **Settings → Pages → Source** and select `Deploy from a branch` (main)
4. Your site will be live at `https://<your-username>.github.io`

## Customizing

Everything lives in `index.html`:

- **Text & translations** — edit the `T` object near the top of the `<script>` block; every language uses the same keys
- **Projects, experience, education, certifications** — edit the corresponding `<section>` markup; card styling is automatic
- **Project links** — GitHub buttons currently point to the profile (`github.com/pronilabh`); swap in individual repository URLs when ready
- **Colors & fonts** — change the CSS variables in `:root`, `[data-theme="dark"]`, and `[data-theme="light"]`

## Tech

Single-file HTML/CSS/JS — no build tools, no frameworks, no dependencies. Fonts (Space Grotesk, Manrope, IBM Plex Mono) loaded from Google Fonts CDN.

## Languages

| Code | Language | Flag |
|------|----------|------|
| EN | English | 🇬🇧 |
| DE | German | 🇩🇪 |
| FR | French | 🇫🇷 |
| PT | Portuguese | 🇧🇷 |
| ES | Spanish | 🇪🇸 |
| HI | Hindi | 🇮🇳 |

Language and theme preferences are stored in `localStorage` and restored automatically on return visits.

## License

© 2026 Nilabh Pandey. All rights reserved.
