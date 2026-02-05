# Quang's Portfolio

Personal portfolio and blog built with [Astro](https://astro.build/).

## Tech Stack

- **Framework:** Astro 5.x (zero JS by default)
- **Styling:** Tailwind CSS v4
- **Content:** Markdown blog with content collections
- **Deployment:** Vercel

## Features

- Dark/light mode with system preference detection
- macOS-style glassmorphism design
- Markdown blog at `/blog/[slug]`
- SEO optimized (sitemap, RSS, JSON-LD)
- View transitions for smooth navigation
- Projects loaded from JSON

## Development

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
npm run preview
```

## Adding Blog Posts

Create a markdown file in `src/content/blog/`:

```markdown
---
title: "Your Post Title"
description: "A brief description"
pubDate: 2026-02-05
tags: ["tag1", "tag2"]
---

Your content here...
```

## Project Structure

```
src/
├── components/     # Astro components
├── content/blog/   # Markdown blog posts
├── data/           # JSON data (projects, site)
├── layouts/        # Page layouts
├── pages/          # Routes
└── styles/         # Global CSS
```

## Deploy to Vercel

1. Push to GitHub
2. Import repo in Vercel dashboard
3. Vercel auto-detects Astro
4. Deploy!

## License

MIT
