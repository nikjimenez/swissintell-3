# Swissintell — Website Redesign

A modern, institutional redesign of [swissintell.ch](https://swissintell.ch) — the Swiss Intelligence Community association (350+ members, est. 2006).

> Static hi-fi landing page. Built with plain HTML/CSS/JS — no build step required.

## Live preview

Open **`Swissintell Landing.html`** in any modern browser, or serve the folder with any static server:

```bash
# Python
python3 -m http.server 8000

# Node
npx serve .
```

Then visit `http://localhost:8000/Swissintell%20Landing.html`.

## What's inside

| Path | Purpose |
|---|---|
| `Swissintell Landing.html` | Main landing page — single file, self-contained markup + styles + scripts |
| `assets/logo.svg` | Official Swissintell wordmark + globe logo |
| `assets/logo.png` | PNG fallback |
| `fonts/calibri-*.ttf` | Calibri family (regular / bold / italic / bold-italic) |
| `index.html` | Redirect to the main file |

## Design system

- **Type:** Calibri (regular / bold / italic) — self-hosted in `/fonts`
- **Palette:** bone white `#FAFAF7`, ink `#0F0F0E`, Swiss red `#DA291C` (accent)
- **Direction:** classic Swiss institutional — editorial rhythm, fine rules, generous whitespace

## Sections

1. Announcement bar + sticky header with EN / FR / DE language switcher
2. Hero — featured upcoming event
3. Discipline marquee strip
4. Stats (members, years, events, languages) with scroll-triggered counters
5. 8 thematic verticals + institutional quote
6. Upcoming events calendar (6 entries)
7. Publications / press review (editorial grid)
8. Member testimonials
9. Membership CTA with pricing tiers
10. Partners grid
11. Footer with newsletter signup

## Animations

- Intro curtain with animated logo + load bar
- Hero split-word reveal
- Featured card slide-in
- IntersectionObserver-driven fade-ups on scroll
- Animated stat counters
- Ken-Burns effect on featured event image
- Respects `prefers-reduced-motion`

## Languages

The header EN/FR/DE switcher swaps the hero copy and persists the choice in `localStorage`. Expand `i18n` in the script block to translate additional strings.

## Notes

- All third-party images are placeholders from Unsplash — replace with real event/member photography for production.
- Based on the April 2026 diagnostic audit (WordPress → custom theme recommendation). The HTML here is intended as a visual direction, to be ported to a WordPress block theme or Elementor build.

## License

Internal / client work. Logo © Swissintell.
