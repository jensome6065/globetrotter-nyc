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
- Color/font choice: I chose a charcoal/off-white base with a taxi-yellow accent (`#f5c518`) plus `Barlow Condensed` for headings and `Inter` for body text; this matches NYC's bold signage energy while keeping long content easy to scan for first-time visitors.
- Claude suggestion I rejected: Claude suggested a subway-line blue accent option, but I rejected it in favor of taxi yellow because blue felt more corporate/tech and less "street-level NYC" for this audience.
- Style that needed correction: My first pass made all section cards feel too heavy and boxed-in, so I softened the visual weight with lighter borders, more internal spacing, and cleaner button contrast to restore the accessible, navigable feel from the wireframe.

## Milestone 3: Flexbox Layout
- Deliberate Flexbox choice: I used `flex-wrap: wrap` with `flex: 1 1 calc((100% - 2.4rem) / 3)` on card grids so desktop stays at a clean 3-up layout while still letting cards reflow naturally at narrower widths.
- Claude mismatch and fix: One generated layout treated the hero and some card groups as mostly stacked blocks on desktop; I changed those sections to true side-by-side flex rows (`.hero` with two columns, plus wrapping grid containers) to match my Milestone 3 plan.
- HTML structure challenge: To make the repeated cards align and size consistently in Flexbox, I introduced dedicated wrapper containers (like `.neighborhood-cards`, `.feature-cards`, `.attraction-grid`, and `.food-grid`) around the `<article>` items, because applying flex directly on mixed section content (headings, paragraphs, and cards together) made spacing and alignment inconsistent.

## Milestone 4: Responsive Design
- Breakpoints used and why: I used 1025px+ (desktop), 768px-1024px (tablet), and 767px and below (mobile) because these ranges map cleanly to common laptop/tablet/phone widths and let my 3-column card layouts step down predictably to 2 columns, then 1 column.
- Mobile layout that needed to feel genuinely different: The header/nav and hero needed more than simple shrinking, so on mobile I prioritized a scan-first order (value text first, image second), allowed nav links to wrap with larger tap areas, and made interactive card actions easier for thumb reach.
- Claude breakpoint suggestion accepted/rejected: I accepted the overall recommendation to use a 3-tier responsive system (desktop/tablet/mobile), but I rejected keeping tablet and mobile behavior too visually similar; I added clearer mobile-specific interaction changes so the phone experience feels intentionally designed rather than just compressed.

## Stretch Features
_Add entries if you implement any stretch features._