# Project Notes

## Structure
- `index.html` — Main site page (actively edited/customized)
- `manifest.json` — PWA manifest (app name, icons, theme)
- `sw.js` — Service worker for offline/PWA support

## Avatar
- Single `images/avatar.webp` is used for both the profile avatar and favicon across all pages

## Cache Busting
- CSS `<link>` tags in `index.html` use a `?v=N` query parameter for cache busting
- Whenever CSS files are modified, bump the version number (1 → 2 → 3 → …) on the affected stylesheet `href`(s)

## PWA
- The site is installable as a Progressive Web App
- `manifest.json` defines the app metadata and icons
- `sw.js` handles caching for offline use
- An install button in the footer prompts supported browsers
