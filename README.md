# FC Barcelona — Més que un club

A four-page FC Barcelona fan site built with HTML and CSS for the
UCD Professional Academy Module 1 web design assessment.

No Javascript, no frameworks.

## Pages

| Page | File | What's on it |
| --- | --- | --- |
| Home | `index.html` | Hero, club intro, feature cards, stats band, motto band |
| History | `history.html` | Timeline of the club's milestones and the "more than a club" story |
| Honours | `honours.html` | Tables of major honours and every European Cup / Champions League final |
| Media | `media.html` | Embedded official Barça video (responsive 16:9) and links to club channels |

## Features

- **Responsive layout** — mobile-first, with breakpoints at 600px (cards two across,
  three-column footer), 768px (two-column hero, four-column stats) and 992px
  (full nav bar, hamburger hidden).
- **CSS-only burger menu** — a hidden checkbox drives the mobile navigation, so it
  works with JavaScript disabled.
- **CSS Grid and Flexbox** — grid for the card, stat and footer rows, flexbox for the
  header and inline layouts.
- **Club colour theme** — blaugrana palette (`--blau #004D98`, `--grana #A50044`,
  gold accent) set as custom properties in `:root`.
- **Semantic HTML** — `header` / `nav` / `main` / `section` / `article` / `footer`,
  captioned `table` elements, `figure` for imagery.
- **SVG imagery** — crest, hero, stadium and trophy illustrations, so everything stays
  sharp at any size and the page stays light.
- **SEO and social meta** — description, keywords, author, robots, theme-colour and
  Open Graph / Twitter card tags on all four pages.

## Accessibility

- Skip-to-content link on every page so keyboard users can tab past the navigation.
- `aria-current="page"` marks the active page in the navigation.
- Section headings that are visually redundant are hidden with a `.visually-hidden`
  class rather than removed, so screen readers still announce them.
- Decorative images use empty `alt`; meaningful images have descriptive `alt` text.
- Visible focus outlines on all interactive elements.
- Animations are disabled under `prefers-reduced-motion: reduce`.
- The honours table scrolls inside its own card on small screens instead of forcing the
  page to scroll sideways.

## Structure

```
.
├── index.html          # Home
├── history.html        # History
├── honours.html        # Honours
├── media.html          # Media
├── css/
│   └── styles.css      # Single stylesheet for the whole site
└── images/
    ├── crest.svg
    ├── hero.svg
    ├── stadium.svg
    └── trophy.svg
```

## Visiting the website

https://iisphilipsii.github.io/module1-webdesign-assessment-fc-barcelona/


## Git workflow

Built one feature at a time. Base styles, then header, navigation,
hero and each home page section in turn, then the responsive breakpoints, then the
three inner pages, then the accessibility passes. The three inner pages were
each built on a feature branch and merged back into main through a pull request.

## Credits and disclaimer

Illustrations are original SVGs made for this project with the help of Claude AI.
The embedded video is an official FC Barcelona clip from the club's own YouTube channel.

This is an unofficial student fan site. It is not affiliated with, endorsed by, or
associated with Futbol Club Barcelona. Club names, crests and trademarks are the
property of their respective owners.

Thank you for taking the time to read.


## Visca Barça, Visca Catalunya


