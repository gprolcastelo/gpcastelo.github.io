# gprolcastelo.github.io

Personal academic site for Guillermo Prol-Castelo, built with [Jekyll](https://jekyllrb.com/) and served via GitHub Pages.

## Structure

- `index.md` — home page (bio, photo, quick links, CV download)
- `portfolio.md` + `_data/portfolio.yml` — featured repos/projects
- `publications.md` + `_data/publications.yml` — publication list
- `blog.md` + `_posts/` — outreach-style blog posts (one Markdown file per post)
- `_data/social.yml` — quick-link URLs (ORCID, Scholar, LinkedIn, Bluesky, GitHub, email)
- `_layouts/`, `_includes/` — page templates
- `assets/` — CSS, images, CV (`assets/cv/CV.pdf`), and other files

## Adding content

- **New blog post**: add `_posts/YYYY-MM-DD-title.md` with `title` front matter.
- **New publication**: add an entry to `_data/publications.yml`.
- **New portfolio project**: add an entry to `_data/portfolio.yml` and drop a figure in `assets/images/portfolio/`.
- **Update quick links / CV**: edit `_data/social.yml` and replace `assets/cv/CV.pdf`.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.
