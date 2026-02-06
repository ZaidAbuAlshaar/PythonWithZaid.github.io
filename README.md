# Zaid.python - تعلم بايثون مع زيد

An interactive Arabic-language platform for learning Python programming, created by **Zaid Abu Alshaar**.

**Live site:** [python.zaiddev.com](https://python.zaiddev.com)

## Overview

Zaid.python is a single-page application (SPA) that teaches Python through 12 structured levels, from basic data types to GUI programming with Tkinter. It includes interactive quizzes, code examples, and FAQ sections -- all available in both Arabic and English.

## Tech Stack

| Component      | Technology                              |
|----------------|-----------------------------------------|
| Markup         | HTML5 (semantic)                        |
| Styling        | Tailwind CSS (CDN) + custom CSS         |
| Scripting      | Vanilla JavaScript (ES6+)               |
| Fonts          | Google Fonts (Tajawal, Inter)           |
| Icons          | Font Awesome 6.0                        |
| Routing        | History API (client-side SPA)           |
| Hosting        | GitHub Pages + custom domain (CNAME)    |

## Folder Structure

```
/
├── index.html              # Main entry point (SPA shell)
├── 404.html                # Custom 404 error page
├── CNAME                   # Custom domain config (python.zaiddev.com)
├── robots.txt              # Search engine crawling rules
├── sitemap.xml             # Sitemap for search engines
├── site.webmanifest        # PWA manifest
├── css/
│   └── style.css           # All custom styles
├── js/
│   └── script.js           # App logic, translations, content, routing
├── assets/
│   ├── img/
│   │   ├── zaid-abu-alshaar.jpg   # Profile photo (optimized)
│   │   └── og-image.jpg           # Social sharing preview image (1200x630)
│   └── icons/
│       ├── favicon.svg            # SVG favicon
│       ├── favicon-32x32.png      # PNG favicon
│       ├── apple-touch-icon.png   # Apple touch icon (180x180)
│       ├── icon-192x192.png       # PWA icon
│       └── icon-512x512.png       # PWA icon (large)
```

## Running Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/ZaidAbuAlshaar/PythonWithZaid.github.io.git
   cd PythonWithZaid.github.io
   ```

2. Serve the files with any static server:
   ```bash
   # Using Python
   python3 -m http.server 8000

   # Or using Node.js (npx)
   npx serve .
   ```

3. Open `http://localhost:8000` in your browser.

## Deployment

- **Hosting:** GitHub Pages (automatically deploys from the main branch).
- **Custom domain:** Configured via the `CNAME` file containing `python.zaiddev.com`.
- **DNS:** Ensure your domain's DNS points to GitHub Pages IPs (see [GitHub docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)).

## SEO Checklist

The following SEO best practices are implemented:

- [x] Unique `<title>` tag
- [x] `<meta name="description">` with relevant content
- [x] `<meta name="author">` set to "Zaid Abu Alshaar"
- [x] `<link rel="canonical">` pointing to the live URL
- [x] `<html lang="ar" dir="rtl">` for proper language declaration
- [x] Open Graph tags (`og:title`, `og:description`, `og:image`, `og:url`, `og:type`)
- [x] Twitter Card tags (`twitter:card`, `twitter:title`, `twitter:description`, `twitter:image`)
- [x] JSON-LD structured data (Person schema + WebSite schema)
- [x] `robots.txt` allowing crawling with sitemap reference
- [x] `sitemap.xml` listing all public pages
- [x] Custom `404.html` error page
- [x] Favicons (SVG, PNG, Apple Touch Icon)
- [x] `site.webmanifest` for PWA support
- [x] Semantic HTML (`<main>`, `<nav>`, `<header>`, `<footer>`, `<section>`)
- [x] Single `<h1>` per page view, logical heading hierarchy
- [x] ARIA labels on interactive elements
- [x] `loading="lazy"` on non-critical images and iframes
- [x] `width`/`height` attributes on images
- [x] `defer` attribute on script loading
- [x] Keyboard focus styles (`focus-visible`)

## Updating Metadata & OG Image

### To update the social sharing preview image:

1. Replace `assets/img/og-image.jpg` with a new image (recommended: 1200x630 pixels, JPEG).
2. Update the `og:image` and `twitter:image` URLs in `index.html` if the filename changes.

### To update the profile photo:

1. Replace `assets/img/zaid-abu-alshaar.jpg` with the new photo.
2. The image reference in `js/script.js` (in the `aboutPage` function) will pick it up automatically.

### To update metadata (title, description):

Edit the `<title>`, `<meta name="description">`, and corresponding OG/Twitter tags in `index.html`.

## License

&copy; 2025 Zaid Abu Alshaar. All Rights Reserved.
