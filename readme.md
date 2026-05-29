# AUSY Landing Page

A high-fidelity, single-page marketing website for **AUSY Fund** — a conceptual ASX-listed Australian income product designed for SMSFs and retail investors.

## Overview

This project is a polished, self-contained landing page that communicates the value proposition of AUSY, a proposed high-yield, tax-efficient investment vehicle with a target distribution yield of ~11.5%.

The live version of this conceptual site is available at **getausy.com**.

The site includes:

- Strong hero messaging and primary CTAs
- Social proof / trust elements (ASX listing, partnership, reporting)
- Detailed feature cards
- Step-by-step "How it Works" section
- Risk disclosures
- Functional waitlist form with validation
- Interactive educational cost base simulators (ROC, DRP, and Clean Exit modelling)

**Important:** This is a conceptual marketing site only. AUSY is not currently listed on the ASX. All yields, figures, and features shown are indicative and subject to change.

## Tech Stack

- **HTML5** + semantic markup
- **Tailwind CSS** (loaded via CDN — no build step)
- **Vanilla JavaScript** (ES6+)
- **Font Awesome 6.5** (CDN icons)
- Google Fonts: Inter + Space Grotesk

No frameworks, bundlers, or build tools are used. The site runs by simply opening `index.html` in a browser.

## Project Structure

```
ausy/
├── index.html     # Complete landing page (all HTML, CSS, JS)
├── readme.md      # This file
└── .git/
```

Everything lives in a single `index.html` file for maximum portability and simplicity.

## Getting Started

### Local Preview

1. Clone or download the repository
2. Open `index.html` directly in any modern browser (Chrome, Firefox, Safari, Edge)

No installation, npm, or build commands required.

### Development

Because Tailwind is loaded via the Play CDN, you can edit `index.html` directly and refresh the browser to see changes. Custom styles and Tailwind overrides live in the `<style>` block near the top of the file.

## Key Features & Interactions

| Feature                    | Description |
|---------------------------|-------------|
| Smooth anchor scrolling   | Custom offset system (`--nav-offset`) prevents content from being hidden behind the sticky navbar |
| Waitlist form             | Client-side validation + success state (submits to Google Form) |
| Educational Simulators    | Interactive modelling tools for ROC tax deferral, DRP reinvestment, and tranche-based exit planning |
| Responsive design         | Mobile-first layout with a collapsible mobile menu |
| Button & shadow polish    | Custom tight shadows on primary CTAs for a premium, grounded feel |
| Keyboard accessibility    | Focus states, escape key support for modals, etc. |

## Customization Guide

### Colors

Primary brand colors are defined in `:root`:

```css
--navy: #0a2540;
--cyan: #00d4ff;
```

The accent cyan (`#00d4ff`) is used extensively for CTAs, icons, and highlights.

### Content

All marketing copy, feature descriptions, and legal disclaimers live directly in `index.html`. Search for section comments (e.g., `<!-- WHY AUSY -->` or the new intent blocks at the top of major sections) to locate specific areas. Many comments have been written to clearly document conceptual/pre-launch intent.

### Form Handling

The waitlist form currently:
- Validates required fields
- Submits to a Google Form (for early interest capture)
- Shows a success state on submission

The form is intentionally lightweight for this conceptual stage. It can be replaced with a more robust backend once the project moves forward.

### Launch Timeline

The site currently references a proposed target timeline of **Q2 2027** in the hero section. All timeline language is illustrative only.

## Browser Support

Designed for modern evergreen browsers. The site uses:

- CSS custom properties
- `backdrop-filter`
- ES6 JavaScript
- Tailwind arbitrary values

## Recent Improvements

- Adopted `getausy.com` as the primary domain
- Added working `Contact` mailto link in footer (`contact@getausy.com`)
- Significantly strengthened meta tags (title, Open Graph, and Twitter Card)
- Updated form placeholders for better Australian tone and domain consistency
- Removed the old Easy Exit Calculator in favour of more educational cost base simulators
- Strengthened compliance language throughout ("proposed", "conceptual", "educational tool only")
- Improved framing of all simulators as generic cost base education tools rather than product-specific demonstrations
- Added and updated multiple HTML comments throughout index.html to clearly document conceptual/pre-launch intent (even non-visible comments)

## Legal & Disclaimers

This is a conceptual marketing website only. It does not represent an offer of any financial product. All content is general information and includes prominent disclaimers consistent with Australian financial services requirements.

The site deliberately uses cautious language ("proposed", "we're building", "conceptual", "educational tool only") to avoid implying that AUSY is a live or guaranteed product. Do not use this site for actual investor communications without proper regulatory review and a Product Disclosure Statement (PDS).

## License

This is a private conceptual project. All rights reserved.

---

Built iteratively as a high-fidelity marketing concept. Feedback and iterations welcome.