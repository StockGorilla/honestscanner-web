# honestscanner.com

Marketing site for the Honest Scanner iOS app. Static HTML + CSS, no build step, deployed via Netlify.

## Structure

```
/
├── index.html              landing page
├── privacy/index.html      privacy policy
├── terms/index.html        terms of use
├── support/index.html      support + FAQ
├── assets/
│   ├── style.css           shared stylesheet
│   ├── hero.png            hero image (add manually)
│   ├── favicon.png         favicon (add manually)
│   └── apple-touch-icon.png (add manually)
├── netlify.toml            Netlify config (headers, publish dir)
├── _redirects              URL redirects
└── README.md
```

## Local preview

```
python3 -m http.server 8000
# or
npx serve .
```

Then open http://localhost:8000.

## Deploy

Netlify auto-deploys on every push to `main`. The domain `honestscanner.com` is managed inside Netlify.

## Editing the legal pages

The privacy policy, terms of use, and support page are HTML files under `/privacy/`, `/terms/`, `/support/`. They're duplicated from `github.com/StockGorilla/honest-scanner-legal` — if that repo's text changes, update these too.

## Design tokens

Matches the iOS app's `src/theme.ts`:

- Paper `#f7f2ea`
- Surface `#fffdf9`
- Ink `#1c1915`
- Muted `#6d675c`
- Green `#1b6b48`
- Green soft `#e5f3ea`
- Serif: Newsreader (Google Fonts) — closest web font to Iowan Old Style
- Sans: system UI (SF Pro on Apple, Segoe UI on Windows)

## Assets to add before launch

- `assets/hero.png` — an iPhone screenshot or product mockup (recommended: use one from the app repo's `design_handoff/appstore/` folder)
- `assets/favicon.png` — 512×512
- `assets/apple-touch-icon.png` — 180×180
- `assets/og.png` — 1200×630 for Open Graph link previews

Copyright © 2026 StockGorilla LLC
