# AUSY Landing Page

A high-fidelity, single-page marketing website for **AUSY Fund** — a conceptual ASX-listed Australian income product designed for SMSFs and retail investors.

## Overview

This project is a polished, self-contained landing page that communicates the value proposition of AUSY, a proposed high-yield, tax-efficient investment vehicle with a target distribution yield of ~11.5%.

The site includes:

- Strong hero messaging and primary CTAs
- Social proof / trust elements (ASX listing, partnership, reporting)
- Detailed feature cards
- Step-by-step "How it Works" section
- Risk disclosures
- Functional waitlist form with validation
- Interactive "Easy Exit Calculator" modal

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
| Waitlist form             | Client-side validation + success state (currently logs submissions) |
| Exit Calculator           | Fully functional modal with live calculations for investment outcomes |
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

All marketing copy, feature descriptions, and legal disclaimers live directly in `index.html`. Search for section comments (e.g., `<!-- WHY AUSY -->`) to locate specific areas.

### Form Handling

The waitlist form currently:
- Validates required fields
- Shows a success state on "submission"
- Logs form data to the console

Replace the `submitWaitlist()` function with real API integration when ready.

### Launch Timeline

The launch target text appears in the trust bar near the top. It was recently updated to **Q2 2027**.

## Browser Support

Designed for modern evergreen browsers. The site uses:

- CSS custom properties
- `backdrop-filter`
- ES6 JavaScript
- Tailwind arbitrary values

## Recent Improvements

- Fixed sticky navbar overlapping section headings on navigation
- Significantly tightened button shadows for better visual hierarchy
- Improved top spacing on the Features section
- Updated launch messaging
- Added precise scroll offset system using a CSS variable

## Legal & Disclaimers

This website contains general information only and does not constitute financial product advice. All content includes prominent disclaimers as required for financial product marketing in Australia.

Do not use this site for actual investor communications without proper regulatory review and a live Product Disclosure Statement (PDS).

## License

This is a private conceptual project. All rights reserved.

---

Built iteratively as a high-fidelity marketing concept. Feedback and iterations welcome.