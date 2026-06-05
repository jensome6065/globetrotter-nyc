MILESTONE 0: PROJECT SETUP
What location are you building this guide for, and why did you choose it?
New York City. I chose NYC because it's where I was born and raised. 

Who is your primary audience? (e.g., first-time visitors, backpackers, families, local residents)
People who don't want to be stuck at the tourist traps. People who want good food. 

What do you want visitors to feel or know after spending 5 minutes on your site?
* accessible, energetic, and navigable *
- Feel excited about what there is to do in NYC, but not overwhelmed
- Understand that the city has so many distinct neighborhoods, each with their own vibes
- Walk away with a list of places they'd genuinely add to their NYC itinerary

What's one design decision — color, layout, or tone — that reflects your destination's identity?
Neutral with one distinct accent color. Clean sections, strong typography, high-contrast visuals

MILESTONE 2: DESIGN INTENT
What color palette reflects your destination? Name three words that describe the feeling.
- Palette: charcoal/black, off-white, soft gray, with one accent color (taxi yellow or subway-line blue).
- Feeling words: energetic, approachable, local.

What typography (heading font / body font) fits your destination's character?
- Heading font: bold, condensed sans-serif style to match NYC signage and fast city energy.
- Body font: clean, highly readable sans-serif for easy scanning on all pages.
- Typography goal: strong hierarchy so users can quickly jump between neighborhoods, food spots, and gallery content.

What's one visual choice that connects to your destination's identity?
- Card-based sections for attractions/food plus image-and-caption gallery blocks to mirror how NYC is explored in neighborhoods and snapshots.

MILESTONE 3: FLEXBOX LAYOUT PLAN
What content does this section contain and how should it be arranged? (e.g., side by side, stacked, grid-like)
- Main sections: hero intro, featured neighborhoods/attractions, food recommendations, and gallery previews.
- Desktop arrangement: hero text + image side by side; cards arranged in flex rows that wrap; footer content in a simple horizontal row.
- Inner section style: each content block uses a reusable card layout with title, image, short description, and link.


How many columns or items should appear in a row at desktop width?
- Hero: 2 columns (text + image).
- Attractions/Food card rows: 3 cards per row.
- Gallery preview row: 3 images per row with captions underneath.


How should that change on a smaller screen?
- Tablet: reduce to 2 cards/images per row, keep readable spacing.
- Mobile: stack to 1 column for hero and cards; nav links can wrap to a second line if needed.
- Keep call-to-action buttons full-width on mobile for easy tapping.


Is there anything about the spacing, alignment, or sizing that's important to the design?
- Use consistent section padding and card gaps to keep the layout clean and scan-friendly.
- Align card content to the top so varying text lengths still look organized.
- Keep max content width centered on large screens so lines do not become too wide.
- Maintain strong contrast, generous whitespace, and consistent image aspect ratios for a polished look.

MILESTONE 4: BREAKPOINTS PLAN
What are the three device sizes you're designing for, and what width defines each breakpoint?
- Desktop: 1025px and up (full multi-column layout).
- Tablet: 768px to 1024px (reduced columns, preserved hierarchy).
- Mobile: 767px and below (single-column, touch-friendly layout).

For each major section of your site, what needs to change at each breakpoint? (e.g., a three-column layout becoming a single column)
- Navigation/header:
  - Desktop: logo + nav links in one row.
  - Tablet: keep single row when possible; reduce horizontal spacing.
  - Mobile: allow nav links to wrap/stack and increase tap target spacing.
- Hero section:
  - Desktop: two columns (intro copy + hero image).
  - Tablet: still two columns but with narrower image and tighter gap.
  - Mobile: stack text above image; center key call-to-action.
- Card grids (neighborhoods, attractions, food):
  - Desktop: 3 cards per row.
  - Tablet: 2 cards per row.
  - Mobile: 1 card per row with full-width buttons/links.
- Gallery:
  - Desktop: 3 images per row.
  - Tablet: 2 images per row.
  - Mobile: 1 image per row with readable captions.
- Footer:
  - Desktop: horizontal layout for grouped links/info.
  - Tablet/Mobile: stack footer content for clarity and spacing.
  
Are there any sections where the mobile experience should feel meaningfully different from desktop, not just smaller?
- Yes: navigation and card actions should be optimized for thumb use on mobile, with wrapped links and larger tap areas.
- The hero should prioritize quick scanning on mobile by showing the value proposition first, then imagery.
- Content order matters more on mobile: show top recommendations earlier so users get useful info within the first screen or two.