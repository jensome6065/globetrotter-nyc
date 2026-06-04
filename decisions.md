# Globetrotter — Decisions Log

## Milestone 0: Setup and Planning
- Destination chosen: NYC
- Primary audience: People who enjoy good food and also don't want to fall for the tourist traps
- One design decision that reflects the destination: Neutral with one distinct accent color
- Wireframe format used (hand-drawn / Figma / other): Claude-generated from my written specs

## Milestone 1: HTML Structure
- Shared structure across all pages: I used consistent `<header>`, `<nav>`, `<main>`, and `<footer>` landmarks so every page can stand alone while keeping navigation predictable.
- Header/logo decision: I moved the logo link out of a paragraph and made it a standalone anchor in the header to keep branding structure cleaner and more semantic.
- Home page (`index.html`): I used `<section>` blocks for hero, neighborhood preview, itinerary, and feature overviews so the content follows a clear "welcome -> discover -> plan" flow from the wireframe.
- Home page refinement: Claude initially gave mostly container-heavy markup; I kept semantic sections and converted repeated content into `<article>` where each item is self-contained.
- Attractions page (`attractions.html`): I kept filters in a dedicated section and grouped repeatable attraction items as `<article>` cards under a single parent section.
- Attractions page heading hierarchy: I changed attraction card titles from `<h2>` to `<h3>` because they are nested under the page/section headings.
- Guide page (`guide.html`): I structured each restaurant as an `<article>` with image, title, location, and description so each entry reads like a standalone recommendation.
- Guide page refinement: Claude generated a placeholder `href="#"` link for Lucali; I replaced it with plain text because there is no official website.
- Gallery page (`gallery.html`): I used `<figure>` and `<figcaption>` for every gallery item so each caption is semantically tied to its image.
- Wireframe-driven choice: The gallery and card layouts in my wireframes directly led me to use repeating semantic patterns (`<article>` for cards and `<figure>` for photos) for consistency across pages.

## Milestone 2: CSS Styling
_Add entries after applying styles._

## Milestone 3: Flexbox Layout
_Add entries after implementing Flexbox._

## Milestone 4: Responsive Design
_Add entries after implementing media queries._

## Stretch Features
_Add entries if you implement any stretch features._