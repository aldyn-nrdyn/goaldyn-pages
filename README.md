# goaldyn-pages

Marketing + support site for **Goaldyn** — a private task, habit, focus and goal
planner for iPhone, by Nrdyn LLC. Free on the App Store, no account, nothing
collected.

Plain static HTML and one stylesheet. No build step, no dependencies, no JavaScript.

Live at **https://goaldyn.nrdyn.com**.

## Pages

| File | URL | Purpose |
|---|---|---|
| `index.html` | `/` | Landing page — features, screenshots, privacy, App Store CTA |
| `support.html` | `/support.html` | FAQ and troubleshooting |
| `privacy.html` | `/privacy.html` | Privacy policy |

## Deploying (Netlify)

The site is deployed on Netlify from this repo: no build command, the publish
directory is the repo root, and `netlify.toml` sets the security and cache
headers. Pushing to `main` deploys.

DNS: `goaldyn.nrdyn.com` is a CNAME to the site's `*.netlify.app` hostname,
managed at Namecheap.

## Assets

- `assets/site.css` — the one stylesheet
- `assets/app-store-badge.svg` — the official Apple badge
- `assets/icon-512.png`, `assets/apple-touch-icon.png`, `assets/favicon-64.png` — app icon sizes
- `assets/og-image.png` — social card
- `assets/screens/` — the five App Store screenshots (640px)

## Notes on the copy

`support.html` and `privacy.html` started life as
`android_app/productivity-hub/docs/{support,privacy}.html` and were refreshed
for the iPhone launch. Keep the privacy page honest about the two-way Apple
Calendar sync and on-device voice entry if those features change.

© 2026 Nrdyn LLC.
