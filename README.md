# khusheel-tech.github.io

Official website for **Khusheel Tech** — served at <https://khusheel-tech.github.io/>
via GitHub Pages (deploys automatically from the `main` branch root).

## Structure

```
.
├── index.html              # Homepage — Khusheel Tech developer landing
├── app-ads.txt             # AdMob app-ads.txt (MUST stay at domain root)
├── 404.html                # Custom not-found page (GitHub Pages serves /404.html)
├── README.md
├── .gitignore
├── assets/
│   ├── icons/              # favicon.svg, favicon-32.png, apple-touch-icon.png
│   ├── logo/               # Brand logo (KT) — SVG master + 1024/512/192 PNG
│   └── social/             # Open Graph / Twitter share card (1200×630)
└── plant-scanner-ai/       # App page + privacy policy (URL is registered — do NOT move)
    ├── index.html
    ├── logo.png
    └── privacy.html
```

## Rules / gotchas

- **`app-ads.txt`** and **`index.html`** and **`404.html`** must stay at the
  repo root — GitHub Pages / AdMob require them there.
- **`/plant-scanner-ai/privacy.html`** is the privacy-policy URL registered in
  Google Play / the app — do not change this path.
- Icons live in `assets/icons/` and are wired via `<link>` tags in each page's
  `<head>`. The brand logo is in `assets/logo/`; the social card is referenced
  by `index.html` as `/assets/social/og-card.png`. Update those links if you
  move files.

## Deploy

Push to `main`; GitHub Pages publishes the root automatically. After changing the
share card, re-scrape with Facebook Sharing Debugger / X Card Validator.
