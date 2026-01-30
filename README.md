# Daisy Xinlei Lin - Personal Website

A modern, fast personal website built with [Astro](https://astro.build/) and [Tailwind CSS](https://tailwindcss.com/).

## Features

- **Modern Design** — Clean, professional layout with dark mode support
- **Blog** — MDX-powered blog with syntax highlighting
- **Responsive** — Mobile-first design that looks great on all devices
- **Fast** — Static site generation for blazing fast load times
- **SEO Ready** — Built-in sitemap, RSS feed, and meta tags
- **Accessible** — Follows web accessibility best practices

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or pnpm

### Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Project Structure

```
personal-website/
├── public/              # Static assets (images, favicon, etc.)
├── src/
│   ├── components/      # Reusable Astro components
│   ├── content/
│   │   └── blog/        # Blog posts (MDX files)
│   ├── layouts/         # Page layouts
│   ├── pages/           # Route pages
│   └── styles/          # Global styles
├── astro.config.mjs     # Astro configuration
├── tailwind.config.mjs  # Tailwind configuration
└── package.json
```

## Writing Blog Posts

Add new blog posts in `src/content/blog/` as `.mdx` files:

```mdx
---
title: "Your Post Title"
description: "A brief description of your post"
pubDate: 2026-01-30
tags: ["AI", "Research"]
---

Your content here...
```

## Customization

### Update Personal Information

1. Edit `src/pages/index.astro` to update your bio, featured work, and publications
2. Edit `src/components/Footer.astro` to update social links
3. Edit `src/components/Header.astro` to update navigation

### Add Your Profile Photo

Place your profile photo at `public/profile.jpg` (recommended size: 400x400px or larger, square aspect ratio)

### Update Colors

Edit `tailwind.config.mjs` to customize the color palette:

```js
colors: {
  primary: { ... },  // Main brand color
  accent: { ... },   // Accent color for highlights
}
```

## Deployment

### GitHub Pages (Recommended)

This repo includes a GitHub Actions workflow for automatic deployment:

1. Push your code to the `main` branch
2. Go to your repo Settings > Pages
3. Under "Build and deployment", select "GitHub Actions"
4. The site will automatically deploy on every push

### Manual Deployment

```bash
npm run build
# Deploy the `dist/` folder to your hosting provider
```

## Tech Stack

- **[Astro](https://astro.build/)** — Static site generator
- **[Tailwind CSS](https://tailwindcss.com/)** — Utility-first CSS
- **[MDX](https://mdxjs.com/)** — Markdown with JSX for blog posts

## License

MIT

---

Built with ❤️ by Daisy Xinlei Lin
