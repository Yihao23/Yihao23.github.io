# Yihao23.github.io

My personal site + blog, hosted free on **GitHub Pages**.

- `index.html` — landing page (intro + links + list of articles)
- `posts/wireless-security-battlemap.html` — an article: the interactive Wireless Security Battlemap

Live at **https://yihao23.github.io** once deployed.

## Deploy in 3 steps (free)

1. **Create the repo** on GitHub named exactly `Yihao23.github.io`
   (Settings → the repo name *must* match your username for the root site.)

2. **Push these files** from this folder:
   ```bash
   cd ~/codespace/Yihao23.github.io
   git init
   git add .
   git commit -m "Personal site + wireless security battlemap"
   git branch -M main
   git remote add origin https://github.com/Yihao23/Yihao23.github.io.git
   git push -u origin main
   ```

3. **Turn on Pages**: GitHub repo → **Settings → Pages** → *Build and deployment* →
   Source = **Deploy from a branch**, Branch = **main / (root)** → Save.
   Wait ~1 minute, then open **https://yihao23.github.io**.

That's it — no server, no cost. `username.github.io` is free; a custom domain
(e.g. `yourname.com`) is optional and costs about $8–12/year.

## Things to edit before/after pushing

- **`index.html`** — the intro paragraph, the About text, and your name.
- The two **"→ point this to the real repo"** links: replace `https://github.com/Yihao23`
  with the actual repo URLs for `gps-security-lab` and `CrossLink` once they are public.
- Add more posts by dropping new `*.html` files into `posts/` and linking them from `index.html`.

## Adding a proper blog later (optional)

For Markdown blog posts with a nicer template, add a static-site generator that
GitHub Pages supports natively:
- **Jekyll** (built into GitHub Pages) — add a `_config.yml` and write posts in `_posts/`.
- or **Hugo** — faster, more themes, build with an Action.

The current setup is plain HTML so it works with zero build step.
