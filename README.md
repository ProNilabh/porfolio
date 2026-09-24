# Nilabh Pandey — Portfolio

Personal portfolio of **Nilabh Pandey**, AI & robotics researcher and MS student at HSLU, Switzerland: IEEE publications, research experience, projects, and a small lab of mini-games built on the research.

**Live:** [nilabhpandey.com](https://nilabhpandey.com) · **GitHub Pages:** [pronilabh.github.io](https://pronilabh.github.io)

One file. No frameworks, no build step, no dependencies: just `index.html` and a photo.

---

## Features

### Interactive
- **Play the Research**: three mini-games based on real projects, with saved high scores, touch and keyboard controls, a 3-2-1 countdown, and auto-pause when you scroll away or switch tabs.
  - **Drone Run**: fly a drone through the gaps between glass towers. Inspired by UAV work at NESAC (ISRO).
  - **Facade Inspector**: find cracked glass panels before time runs out while ignoring reflections. You're scored like a classifier, with precision, recall and F1. Inspired by the IEEE I2CACIS 2025 paper.
  - **Target Lock**: keep a servo-driven turret's crosshair on a jinking drone inside a YOLO-style bounding box. Inspired by the drone detection & tracking project.
- **Interactive terminal**: the Skills section is a working shell (`help`, `projects`, `skills ml`, `play drone`, `lang de`…) with Tab completion and command history.
- **Command palette**: `Ctrl K` / `⌘K` jumps to any section, switches language or theme, copies the email, saves the contact card, shares the page, starts a game or saves the page as a PDF.
- **Experience tabs**, **filterable projects** with "Show all", and **skills tabs**.
- **Copy BibTeX** on each paper, **copy email**, **save contact (.vcf)** and **share** (native share sheet on phones; copies the link on desktop).
- Easter eggs: a signature in the browser console, and the Konami code (↑ ↑ ↓ ↓ ← → ← → B A) unlocks a gold drone.

### Languages & themes
- **6 languages**: English, German, French, Portuguese, Spanish and Hindi. Every visible string is translated, including the games and the terminal.
- Detects the browser language on the first visit and remembers the choice.
- **Dark / light theme**, remembered, with a theme-aware starfield background.
- Flags are inline SVG, because Windows can't display emoji flags.

### Quality
- Responsive from 320px phones to wide screens. Mobile gets a full-screen menu, swipeable certificates and 16px inputs so iOS doesn't zoom in.
- Accessible: keyboard navigation everywhere, ARIA tabs and dialogs, visible focus, a skip link, and support for `prefers-reduced-motion`.
- SEO: Open Graph and Twitter cards, a canonical URL, JSON-LD `Person` schema (education, expertise, profiles) and a translated meta description.
- **Print / Save as PDF** produces a clean, resume-style page.
- Content stays readable with JavaScript disabled.
- No analytics and no cookies. Preferences and high scores stay in the visitor's own `localStorage`.

## Sections

Hero · About · Experience · Education · Publications · Projects · Skills · Certifications · Lab · Contact

## Keyboard shortcuts

| Keys | Action |
|---|---|
| `Ctrl K` / `⌘K` | Open the command palette |
| `Esc` | Close the palette or menu · pause a game |
| `Space` / `↑` | Drone Run: climb (or click / tap) |
| Arrow keys + `Enter` | Facade Inspector: move and select a panel (or click / tap) |
| Arrow keys | Target Lock: move the crosshair (or mouse / drag) |
| `Tab` · `↑` `↓` · `Ctrl L` | Terminal: autocomplete · history · clear |

## Terminal commands

| Command | What it does |
|---|---|
| `help` | List all commands |
| `whoami` | Short introduction |
| `ls`, `cd <section>` | List sections / scroll to one (`cd projects`) |
| `experience`, `projects`, `papers`, `education` | Print that section in the current language |
| `skills <category>` | Show a skill group: `lang`, `ml`, `cloud`, `hw`, `dom`, `spoken` |
| `contact`, `email` | Show contact details / copy the email address |
| `hire` | Open a new email |
| `play <game>` | Start `drone`, `facade` or `track` |
| `theme [dark\|light]` | Switch the theme |
| `lang <code>` | Switch language: `en`, `de`, `fr`, `pt`, `es`, `hi` |
| `cv` | Save the page as a PDF |
| `neofetch`, `date`, `echo`, `history`, `clear` | The usual |

## Customizing

Everything lives in `index.html`:

- **Text & translations**: the `T` object at the top of the `<script>`. Every language uses the same keys, so edit all six.
- **Sections**: edit the matching `<section>` markup. Cards, tabs and reveals style themselves.
- **Games**: the `INTERACTIVE LAB` block in the script. The difficulty constants (speed, gap size, round length) sit at the top of `makeDrone`, `makeFacade` and `makeTrack`.
- **Terminal commands**: the `INTERACTIVE SHELL` block.
- **BibTeX entries**: the `COPY BIBTEX` block. Add the full co-author list there.
- **Contact card**: `saveVCard()` in the `SAVE CONTACT (.vcf) + SHARE` block.
- **Project links**: the GitHub buttons point to the profile (`github.com/pronilabh`). Swap in individual repository URLs when they're public.
- **Colors & fonts**: the CSS variables in `:root`, `[data-theme="dark"]` and `[data-theme="light"]`.

## Languages

| Code | Language | Notes |
|---|---|---|
| EN | English | Default |
| DE | German | Swiss Standard German spelling (`ss`, no `ß`) |
| FR | French | |
| PT | Portuguese | Portugal flag |
| ES | Spanish | |
| HI | Hindi | Devanagari script |

## Tech

Single-file HTML, CSS and vanilla JavaScript, with Canvas 2D for the games and the starfield. Fonts: Space Grotesk, Manrope and IBM Plex Mono, loaded from Google Fonts.

## License

© 2026 Nilabh Pandey. All rights reserved.
