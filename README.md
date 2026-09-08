# goaldyn_website

The marketing and support site for **Goaldyn** — a private task, habit, focus and goal planner for
iPhone, by Nrdyn LLC. Free on the App Store, no account, nothing collected.

Plain static HTML and one stylesheet. No build step, no dependencies, no JavaScript.

**Live at [goaldyn.nrdyn.com](https://goaldyn.nrdyn.com).**

## Pages

| File | URL | Purpose |
|---|---|---|
| `index.html` | `/` | Landing page — features, screenshots, privacy, App Store CTA |
| `support.html` | `/support.html` | FAQ and troubleshooting |
| `privacy.html` | `/privacy.html` | Privacy policy |

`robots.txt` and `sitemap.xml` are hand-written and list those three pages. If a page is added,
add it to the sitemap too — nothing generates it.

## Assets

| Path | What |
|---|---|
| `assets/site.css` | The one stylesheet |
| `assets/app-store-badge.svg` | Apple's official badge — do not redraw or recolour it |
| `assets/icon-512.png`, `apple-touch-icon.png`, `favicon-64.png` | App icon sizes |
| `assets/og-image.png` | Social preview card |
| `assets/screens/` | The five App Store screenshots, 640 px |

`.nojekyll` stops GitHub Pages from running the files through Jekyll, which would otherwise ignore
anything beginning with an underscore.

## Deploying

`netlify.toml` sets the security and cache headers: no build command, publish directory is the repo
root. Push to `main` and the connected site deploys.

**Which repo actually deploys is worth checking before you rely on this.** The site has also lived
at `aldyn-nrdyn/goaldyn-pages`, and `goaldyn.nrdyn.com` is a CNAME to a `*.netlify.app` hostname
managed at Namecheap. Only one repo can be the Netlify source. If this one is not it, pushing here
changes nothing that is live — point Netlify at this repo first, then retire the other, so there is
exactly one copy the search engines and the App Store listing can agree on.

## Notes on the copy

`support.html` and `privacy.html` were refreshed from the predecessor app's docs for the iPhone
launch. **Keep the privacy page honest**: it makes specific claims about two-way Apple Calendar sync
and on-device voice entry, and those have to stay true of the shipped app. A privacy policy that
describes a version of the app that no longer exists is the one page here that can cause real harm.

© 2026 Nrdyn LLC.
