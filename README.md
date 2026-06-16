# TuneUp.ai website

A simple, Markdown-based revival of the old tuneup.ai / ascar.io site,
built with [Jekyll](https://jekyllrb.com/) + the
[minima](https://github.com/jekyll/minima) theme and hosted on GitHub Pages.

## Editing

Everything is plain Markdown — just edit and push:

| File | Page |
|------|------|
| `index.md` | English landing page (`/`) |
| `zh/index.md` | Chinese landing page (`/zh/`) |
| `pilot.md` | Pilot Benchmark Framework (`/pilot/`) |
| `assets/img/` | images |
| `assets/pdf/` | white paper & papers |
| `_config.yml` | site title, nav, theme |

## Publishing to GitHub Pages

1. Create a new **public** repo on GitHub (e.g. `tuneup-site`).
2. Push this folder:
   ```bash
   git init
   git add .
   git commit -m "Initial Jekyll site"
   git branch -M main
   git remote add origin git@github.com:USERNAME/tuneup-site.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   pick `main` / `/ (root)`, save.
4. The site goes live at `https://USERNAME.github.io/tuneup-site/` in a minute or two.

> If you publish under a subpath like `/tuneup-site/`, set `baseurl: "/tuneup-site"`
> in `_config.yml` so links resolve correctly. For a user page
> (`USERNAME.github.io`) or a custom domain, leave `baseurl` empty.

### Custom domain (optional)
To use `tuneup.ai` again, add a `CNAME` file containing `tuneup.ai`, point the
domain's DNS at GitHub Pages, and set it under Settings → Pages.

## Local preview (optional)

Requires Ruby:
```bash
bundle install
bundle exec jekyll serve
# open http://localhost:4000
```
