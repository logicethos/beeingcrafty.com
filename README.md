# beeingcrafty.com

Static website for [Bee-ing Crafty](https://beeingcrafty.com), a handmade-goods business. Logic Ethos Ltd hosts the site.

The live files are in `public/`: a single page (`index.html`) and the logo (`beeing_crafty.jpg`).

## Preview locally

From this directory:

```bash
python3 -m http.server 8080 --directory public
```

Then open http://localhost:8080/

## Cloudflare Pages

This repo is meant to be served by Cloudflare Pages.

- **Framework preset:** None
- **Build command:** leave empty (no build)
- **Build output directory:** `public`
- **Production branch:** `main`

After a push to `main`, Pages publishes automatically.

## Email and DNS

Mail for `@beeingcrafty.com` is handled by `mx.logicethos.com`. The `mail` hostname must stay as a DNS-only A record pointing at the mail server, and must not be proxied through Cloudflare.
