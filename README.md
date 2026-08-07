# Top 10 Parks in Toowoomba — Version 1

A single-page static site listing the ten best parks in Toowoomba, QLD. Built with plain HTML and CSS — no build tools, no JavaScript, no dependencies.

## Folder structure

```
top10-parks-toowoomba/
├── index.html              ← the entire site (one page)
├── css/
│   └── styles.css          ← all styling
├── images/
│   ├── favicon.svg         ← placeholder site icon
│   └── parks/
│       ├── 01-queens-park.svg
│       ├── 02-laurel-bank-park.svg
│       ├── ... (10 total)  ← placeholder photos, one per park
├── robots.txt               ← tells search engines they can crawl the site
├── sitemap.xml               ← tells search engines what pages exist
└── README.md                 ← this file
```

## Running it locally

No installation needed. Two options:

1. **Simplest:** double-click `index.html` and it opens in your browser.
2. **Recommended** (avoids a couple of minor local-file quirks): serve it with a tiny local server from inside the project folder:
   - Python: `python3 -m http.server 8000` → open `http://localhost:8000`
   - Node: `npx serve` → open the URL it prints

## Deploying to GitHub Pages

1. Create a new GitHub repository (e.g. `top10-parks-toowoomba`).
2. Upload every file in this folder to the repository, keeping `index.html` at the repository root (not inside a subfolder).
3. In the repository, go to **Settings → Pages**.
4. Under "Build and deployment," set **Source** to "Deploy from a branch," **Branch** to `main`, folder `/ (root)`.
5. Save. GitHub publishes the site at `https://YOUR-USERNAME.github.io/top10-parks-toowoomba/` within a minute or two.
6. **Important:** once you know your real URL, replace every `TODO` placeholder (search for `YOUR-GITHUB-USERNAME`) in `index.html`, `robots.txt`, and `sitemap.xml`.

## Assumptions made

- The ten parks and their general facilities were drawn from public sources (council/tourism listings) to make the placeholder content realistic rather than invented from nothing.
- The ranking order (1–10) is a reasonable draft, not a claim based on any survey — you should feel free to reorder it based on your own judgement.
- No custom domain, analytics, or AdSense code is wired in yet, per the approved specification.
- Descriptions are original placeholder copy in the right format (4 sentences) — not final, fact-checked content.

## Content still needed before public launch

- [ ] Real photos for all 10 parks (currently branded gradient placeholders)
- [ ] Fact-checked, finalised descriptions for each park
- [ ] Your own final call on the ranking order
- [ ] Real GitHub username / domain in place of every `TODO` placeholder URL

## Deferred to future versions

Per the approved specification: interactive map, filters, reviews/ratings, search, individual park pages, custom domain, Google AdSense integration, expanded analytics, and growing beyond the top 10. Two ad placeholder slots (side + bottom) are already reserved in the layout for when AdSense is ready.
