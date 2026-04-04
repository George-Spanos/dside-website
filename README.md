# dside studio

Website for dside studio — a two-person design and engineering studio.

## Team

**George Spanos** — Engineering. Front-end architecture, team leadership, full-stack delivery. 10+ years across banking (Bank of Greece, National Bank of Greece), government (GOVUK via Trasys), and product studios (Moby IT, TRG).

**Katerina Spatharou** — Design. UI/UX, design systems, graphic design. Product design at Viva.com (B2B banking platform), print and digital at Psichogios Publications, and product design at Moby IT.

## Tech stack

Single-file HTML/CSS site. No build tools, no framework, no dependencies beyond two Google Fonts (Inter, JetBrains Mono).

## Project structure

```
dside studio website/
├── team-cvs/            # Team CVs (not committed to git)
└── site/                # Git repo root
    ├── index.html       # The entire website
    └── README.md
```

## Running locally

Any static file server works. Examples:

```bash
# Python
python3 -m http.server 8080

# Node
npx serve .

# Or just open index.html directly in a browser
open index.html
```

## Design decisions

**Dark theme** with a warm amber accent (#c9a96e). The palette is intentionally muted — near-black backgrounds, soft off-white text.

**Vinyl motif** — dside studio draws from the founders' shared interest in music and vinyl records. This shows up in three subtle, CSS-only ways:
- The "d" in the logo sits inside a disc with concentric groove rings
- Section headers trail off with a dashed line evoking turntable grooves
- The footer contains a small vinyl dot

**Semantic HTML** — the site uses `header`, `main`, `footer`, `nav`, `article`, `section`, `address`, `dl`/`dt`/`dd`, `time`, `mark`, and `small` instead of generic divs. This improves accessibility, SEO, and maintainability.

**No JavaScript** — the site is pure HTML and CSS. No animations, no parallax, no scroll hijacking, no cookie banners.

## Deployment

The site is a single HTML file. It can be deployed anywhere that serves static files: GitHub Pages, Netlify, Vercel, Cloudflare Pages, or a plain web server.

For GitHub Pages, enable it in the repo settings under Pages → Source → Deploy from branch → `main` → `/ (root)`.

## License

All rights reserved © 2026 dside studio.
