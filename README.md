# Resume Website — CSS Write-up
**Shubhank Srivastava** · shubhank9999@gmail.com

**GitHub Pages:** https://thoioyou.github.io/Resume-Website

---

## What I Built

I built my personal resume website using HTML and CSS. Instead of the usual card grid layout, I went with an editorial magazine style — big serif typography, a dark background with an off-white (#e8e6e0) colour scheme, and animated sections that reveal as you scroll.

---

## CSS Improvements Made

- **Google Fonts** — Imported Playfair Display for headings, DM Mono for labels, and DM Sans for body text. The serif + mono pairing gives it an editorial feel.

- **CSS Variables** — All colours and fonts defined in `:root` (e.g. `--ink`, `--paper`, `--mid`), keeping the theme consistent without repeating values.

- **position: fixed** — Used for the navbar so it stays pinned to the top while scrolling, with a blur background that fades in after 60px of scroll.

- **Flexbox & CSS Grid** — Flexbox for the navbar, stats row, and contact section. Grid for the hero layout, education columns, and proficiency table.

- **@keyframes animations** — Hero name slides up on load, a role ticker scrolls horizontally at the bottom of the hero, and a scroll hint line pulses on the right.

- **Transitions & hover effects** — Nav links get a sliding underline, cards shift on hover, contact rows indent, and skill tags invert colour — all using `transition`.

- **Scroll reveal** — Sections start at `opacity: 0` and animate into view using `IntersectionObserver` toggling a CSS class.

- **::before pseudo-element** — A giant faint "SS" watermark sits in the hero background to fill the page visually.

- **@media queries** — Two breakpoints (900px and 680px) collapse grids to single column and swap the desktop nav for a hamburger menu. Font sizes scale with `clamp()`.

---

## Semantic HTML Used

`<header>`, `<nav>`, `<section>`, `<article>`, `<footer>` — used throughout instead of generic divs.

---

## What I Learnt

This project taught me more than I expected. Getting the scroll reveal working was the most satisfying part. I also spent a lot of time on typography — pairing fonts and getting the spacing right made the biggest difference to how the site looked overall.
