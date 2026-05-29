# Capstone Next.js Templates

A responsive SaaS landing page template built with static HTML, Tailwind CSS v4, Preline UI, and a small amount of custom JavaScript. The project presents a Next.js/SaaS starter style interface, but the current implementation is a static front-end template with no framework runtime required.

[Live Demo](https://capstone-nextjstemplates-ukl7.vercel.app/)

## Author and Usage

This project was built with Nguyễn Đức Đạt.

Project này được xây dựng với Nguyễn Đức Đạt. Dự án phục vụ cho việc học tập và không sử dụng cho mục đích thương mại.

## Overview

This template is designed for SaaS, startup, product, and software landing pages. It includes a complete marketing homepage, supporting pages, dark mode, responsive navigation, animated sections, pricing cards, testimonials, FAQ, contact form UI, blog cards, and reusable visual assets.

## Features

- Responsive multi-section SaaS homepage
- Light and dark theme support with local storage persistence
- Sticky header with mobile navigation
- Hero, brand strip, features, about, integrations, tabs, CTA, FAQ, testimonials, pricing, contact, blog, and footer sections
- Additional static pages for blog, documentation, and support
- Scroll-triggered animations using `IntersectionObserver`
- Testimonials carousel powered by Slick Carousel
- Preline UI components for dropdowns, tabs, and collapsible navigation
- Tailwind CSS v4 build pipeline

## Tech Stack

- HTML5
- CSS3
- Tailwind CSS v4
- Tailwind CLI
- Preline UI
- JavaScript
- jQuery and Slick Carousel via CDN
- Font Awesome via CDN
- Google Fonts

## Project Structure

```text
.
|-- index.html
|-- views/
|   |-- blog.html
|   |-- doc.html
|   `-- support.html
|-- src/
|   |-- css/
|   |   |-- input.css
|   |   |-- output.css
|   |   `-- style.css
|   |-- images/
|   `-- js/
|       |-- main.js
|       `-- preline.js
|-- public/
|   |-- brand/
|   |-- hero/
|   |-- icon/
|   |-- img_qt/
|   |-- logo/
|   `-- shape/
|-- package.json
`-- package-lock.json
```

## Getting Started

### Prerequisites

Install Node.js and npm before running the build scripts.

### Installation

```bash
npm install
```

### Development

Start Tailwind in watch mode:

```bash
npm start
```

Then open `index.html` in a browser or serve the folder with any static file server.

### Production Build

Generate a minified Tailwind output file:

```bash
npm run build
```

The generated stylesheet is written to:

```text
src/css/output.css
```

## Available Scripts

| Command | Description |
| --- | --- |
| `npm start` | Watches `src/css/input.css` and rebuilds `src/css/output.css` during development. |
| `npm run build` | Builds and minifies the Tailwind CSS output for production. |

## Pages

- `index.html` - Main SaaS landing page
- `views/blog.html` - Blog listing page
- `views/doc.html` - Documentation page
- `views/support.html` - Support page

## Customization

- Update page content directly in `index.html` and files inside `views/`.
- Edit Tailwind theme tokens in `src/css/input.css`.
- Add or override custom section styles in `src/css/style.css`.
- Replace logos, icons, hero artwork, and brand assets inside `public/`.
- Update interactive behavior in `src/js/main.js`.

## Deployment

This is a static front-end project, so it can be deployed to any static hosting provider such as Vercel, Netlify, GitHub Pages, Cloudflare Pages, or a traditional web server.

Recommended deployment flow:

```bash
npm install
npm run build
```

Deploy the project folder after the production CSS has been generated.

## Notes

- The repository name and page title reference Next.js, but there is currently no Next.js application structure, React code, or server-side runtime in this project.
- External assets and scripts are loaded from CDNs for Font Awesome, Google Fonts, jQuery, and Slick Carousel.
- Form elements are UI-only and do not submit to a backend by default.

## License

No license file is currently included. Add a license before publishing or distributing this project publicly.
