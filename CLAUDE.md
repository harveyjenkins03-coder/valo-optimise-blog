# Valo Optimise Blog — Claude Code Context

## What this project is
The blog for Valo Optimise at blog.valooptimise.com — static HTML articles covering Valorant performance, PC optimisation, and gaming guides. Drives ad revenue and app downloads.

## Tech stack
- **Format**: Static HTML files in `posts/`
- **Hosting**: Cloudflare Pages
- **SEO**: sitemap.xml, robots.txt, Google verification
- **No build step** — raw HTML, deployed on push to master

## Structure
```
posts/             — HTML blog articles (one file per post)
index.html         — Blog homepage
sitemap.xml        — SEO sitemap
robots.txt         — Crawler rules
_headers           — Cloudflare headers config
_redirects         — Cloudflare redirect rules
reddit_posts.md    — Reddit promotion drafts
```

## Team & Permissions
- **harveyjenkins03-coder** (Harvey) — Owner. Full access.
- **adamtraveltech-maker** (Adam) — Marketing Lead. Content author.

### Adam's scope (ENFORCED)
Adam works on: blog posts in `posts/`, reddit_posts.md, and content assets.
Adam must NOT modify: _headers, _redirects, index.html structure, sitemap.xml, robots.txt, or Cloudflare config.
All changes go through Pull Requests to `master` — direct pushes are blocked.

## Writing a new blog post
1. Create a new HTML file in `posts/` following the naming convention: `topic-keywords-2026.html`
2. Match the existing HTML template structure (head meta tags, header, article body, footer)
3. Include SEO meta tags: title, description, keywords, og:title, og:description
4. Open a Pull Request for review

## Rules
- All content must be original — no copy-paste from other sites
- Include proper meta tags for SEO on every post
- Never commit credentials, API keys, or internal business information
- Never reference Valo Security, bug bounty work, or pentesting
- Keep articles factual — no misleading performance claims
- All PRs require review before merge (branch protection enforced)
- Never modify infrastructure files (_headers, _redirects, robots.txt) without Harvey's approval
