# Pointless Websites

A small collection of single-serving, deliberately pointless websites.
Static HTML/CSS/JS. No build step, no dependencies, no tracking.

## Structure

```
/                index.html      One word. Tap it.  (the public face)
/wealth/         index.html      $10k vs $1M vs $1B — a true-to-scale tunnel
                 hero.jpg        social/share image
                 grid.jpg        "every dot is a million" field
robots.txt
sitemap.xml
```

`/wealth/` is intentionally unlisted: it carries `noindex` and is not in the
sitemap. It is reached by tapping the word on the home page, which sets a
`w=1` cookie; visiting it directly without that cookie bounces back to `/`.

## Deploy (Cloudflare Pages)

1. Connect this repo to a new Cloudflare Pages project.
2. Framework preset: **None**. Build command: *(empty)*. Output directory: `/`.
3. Add the custom domain `pointless-websites.com` in the Pages project.

Because everything is static, "direct upload" of this folder works too.
