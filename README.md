# rosspower.ai

The personal site for **Ross Power** — AI keynote speaker, workshop facilitator
and mentor. A single, self-contained static page (HTML + inline Tailwind CSS +
vanilla JS). No build step, no dependencies.

## Structure

```
index.html   The entire site (markup, styles and scripts inlined)
```

## Develop locally

It's just a static file, so open it directly or serve it:

```bash
# open directly
open index.html

# or serve on http://localhost:8000
python3 -m http.server 8000
```

## Hosting

Deployed on **Cloudflare Pages**, connected to this GitHub repo. Every push to
`main` triggers an automatic deploy. The site is served at
[rosspower.ai](https://rosspower.ai) via a custom domain on the Cloudflare zone.

### Cloudflare Pages settings

| Setting | Value |
| --- | --- |
| Production branch | `main` |
| Build command | _(none)_ |
| Build output directory | `/` |

## Editing content

All copy and the repeated card/marquee/carousel content live in the `<script>`
block near the bottom of `index.html` (`topics`, `formats`, `tags`, the marquee
lists and the carousel builders). Static copy (hero, about, CTA) is inline in
the markup above it.
