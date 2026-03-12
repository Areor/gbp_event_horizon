# EVENT HORIZON
### Deep Space News Network

> *Where the observable universe ends.*

A fully static, single-file HTML space news website inspired by the SpaceX design language — brutally minimal, precision typography, data-dense layouts with animated visuals.

---

## Getting Started

1. Download `event-horizon.html`
2. Open it in any modern browser
3. No server, no install, no dependencies required

```bash
# Or serve locally with Python
python3 -m http.server 8080
# → open http://localhost:8080/event-horizon.html
```

---

## Cloning the Repository

```bash
# Clone
git clone https://github.com/Areor/event-horizon.git

# Navigate into the folder
cd event-horizon

# Open the site
open event-horizon.html
```

---

## Features

### Design & UI
- **SpaceX-inspired aesthetic** — Barlow Condensed typography, monochromatic palette, military-grade precision
- **Dark / Light Mode** — full theme toggle with smooth CSS variable transitions across all elements
- **Animated Solar System Hero** — 6 orbiting planets around a black hole with rotating accretion disk and gravitational wave pulses
- **Live UTC Clock** — real-time UTC display in the topbar
- **Scrolling News Ticker** — continuous breaking news feed in the header

### Navigation
- **Left sidebar** — icon-only nav with hover tooltips linking to all five sections
- **Right sidebar** — 5 fake advertising banners (Starlink, Meade Instruments, Virgin Galactic, NASA Citizen Science, Stellarium)
- **Smooth scroll** — animated scroll to sections via nav buttons

### Content Sections

| Section | Description |
|---|---|
| 📡 Breaking News | Featured story + 3 news cards with Breaking / Exclusive / Update tags |
| 🌌 Astronomical Event Tracker | Timeline with live/upcoming events and countdown |
| 🚀 Mission Control | 6 active space missions with status, stats and progress bars |
| 🔭 Deep Space Discoveries | 6 discovery cards: black holes, gravitational waves, exoplanets and more |
| 🌙 Night Sky Guide — Tonight | Interactive sky dome + visibility table for tonight's objects |

---

## Tech Stack

| Technology | Usage |
|---|---|
| HTML5 | Structure |
| CSS3 | Layout (CSS Grid), animations, CSS variables for theming |
| Vanilla JavaScript | Clock, sky dome, theme toggle, smooth scroll |
| Google Fonts | Barlow Condensed + Barlow |

**No frameworks. No dependencies. Zero build steps.**  
100% single-file — save as `.html`, open in browser.

---

## File Structure

```
event-horizon.html   ← entire website (HTML + CSS + JS in one file)
README.md            ← this file
```

---

## Customisation

### Switch default theme
Change the `data-theme` attribute on the `<html>` tag:
```html
<html data-theme="dark">   <!-- default dark -->
<html data-theme="light">  <!-- default light -->
```

### Add news stories
Add a `.nc` card inside `.ng` in the Breaking News section:
```html
<div class="nc">
  <div class="ntag tr">⚡ Breaking</div>
  <div class="nhl">Your Headline Here</div>
  <div class="nb">Body text goes here.</div>
  <div class="nm"><span>Source</span><span>Just now</span></div>
</div>
```

### Add ticker items
Duplicate a `.tick-item` in both the first and second half of `.tick-inner` (the second half is needed to keep the infinite loop seamless):
```html
<span class="tick-item"><span class="tick-dot"></span>Your ticker text here</span>
```

---

## Browser Support

| Browser | Status |
|---|---|
| Chrome 90+ | ✅ Full support |
| Firefox 88+ | ✅ Full support |
| Safari 14+ | ✅ Full support |
| Edge 90+ | ✅ Full support |

> Requires support for CSS Grid, CSS custom properties, Canvas API, and `conic-gradient`.

---

## Design Principles

- **No colour except function** — red is reserved for live/breaking signals only
- **Typography does the work** — Barlow Condensed at varying weights replaces icons and decorative elements
- **1px borders, no shadows** — flat, precise, no depth tricks
- **Content density over whitespace** — data-heavy layouts inspired by mission control interfaces

---

## License

Free to use, modify and distribute for personal and commercial projects.
All news content is fictional and for demonstration purposes only.
Advertisement slots are placeholder/fake — no real advertisers involved.

---

*Built with Claude · Event Horizon © 2026*
