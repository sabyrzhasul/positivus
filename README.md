# Positivus

A static landing page for a digital marketing agency, built with semantic HTML and Sass. Based on a [Figma community design](https://www.figma.com/community).

## Preview

![Project Preview](src/assets/images/preview.png)

## Features

- Fully responsive single-page layout with mobile navigation overlay
- Sections: Hero, Services, Case Studies, Working Process, Team, Testimonials, Contact Form
- Accordion-based "Working Process" section using native `<details>` elements
- Testimonials slider with pagination controls
- Newsletter subscription form in the footer
- BEM methodology for CSS class naming
- Mobile-first responsive design with burger menu (`<dialog>` element)

## Tech Stack

- **HTML5** — semantic markup
- **Sass (SCSS)** — modular stylesheets
- **gh-pages** — deployment to GitHub Pages

## Project Structure

```
src/
├── assets/
│   ├── fonts/          # Custom web fonts
│   └── images/         # SVG icons, backgrounds, team/partner logos
├── styles/
│   ├── base/           # Reset, variables, fonts, global styles, utilities
│   ├── components/     # Reusable UI components (buttons, cards, forms, etc.)
│   ├── helpers/        # Sass mixins and media query helpers
│   ├── layouts/        # Header, footer, grid, section layouts
│   ├── sections/       # Page section styles (hero, services, team, etc.)
│   ├── main.scss       # Main entry point that imports all partials
│   └── main.css        # Compiled CSS output
└── index.html          # Single-page HTML
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (for Sass compilation and deployment)

### Installation

```bash
npm install
```

### Development

Compile Sass and watch for changes:

```bash
npm run sass:watch
```

Then open `src/index.html` directly in a browser.

### Production Build

Compile Sass once:

```bash
npm run sass:build
```

## Scripts

| Script | Description |
|---|---|
| `npm run sass:build` | Compile `main.scss` to `main.css` |
| `npm run sass:watch` | Watch for SCSS changes and recompile automatically |
| `npm run deploy` | Build CSS and deploy the `src/` directory to GitHub Pages |

## Deployment

The project is configured for deployment to [GitHub Pages](https://pages.github.com/) using the `gh-pages` package:

```bash
npm run deploy
```

This runs `sass:build` as a pre-deploy step, then publishes the `src/` directory.

**Live site:** [https://sabyrzhasul.github.io/positivus](https://sabyrzhasul.github.io/positivus)

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m 'Add my feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a Pull Request

## License

This project is licensed under the [ISC License](https://opensource.org/licenses/ISC).
