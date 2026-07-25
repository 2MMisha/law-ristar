# law.ristar.co

Legal documents (Privacy Policy, Terms of Use, Accessibility Statement) for the
Rising Star website, in Hebrew, English, and Russian.

## Structure

```
.
├── index.html      # root — detects browser language, redirects to /he/, /en/, or /ru/
├── he/index.html    # Hebrew (RTL) — default/fallback language
├── en/index.html    # English
├── ru/index.html    # Russian
├── 404.html         # simple not-found redirect back to /
└── CNAME             # GitHub Pages custom domain: law.ristar.co
```

## Deploying (GitHub Pages)

1. Push this repo to GitHub.
2. In the repo's **Settings → Pages**, set the source to the branch/folder
   this content lives in (e.g. `main` / root).
3. GitHub Pages will read `CNAME` automatically and serve the site at
   `law.ristar.co`, as long as your DNS (A/ALIAS/CNAME records at your
   registrar) points at GitHub Pages.
4. Each page is self-contained (inline CSS, no build step) — just static
   HTML, so no build pipeline is required.

## Editing

Each language page is a single standalone HTML file with three sections:
`#privacy`, `#terms`, `#accessibility`. Update the same section in all three
language files when the underlying facts change (address, phone, business
details, etc.) to keep them in sync. The "last updated" date near the top of
each section should be bumped whenever content changes.

## Accessibility widget

All three pages load the [Tabnav](https://tabnav.com/accessibility-widget)
script, with `language` and `widgetLocation` set per page (Hebrew is RTL, so
its widget button sits on the left; English/Russian sit on the right).

## Notes

- Content was rewritten for clarity (not just translated) from the previous
  Hebrew-only version. Facts are unchanged, but a legal review before this
  fully replaces the live site is recommended.
- Fonts: Arimo (body) + Montserrat (headings), loaded from Google Fonts.
