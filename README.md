# fatemehdoudi.github.io

Source for my personal academic website: **[fatemehdoudi.github.io](https://fatemehdoudi.github.io)**.

I'm Fatemeh Doudi, a Ph.D. student in Electrical and Computer Engineering at Texas A&M University. The site hosts my bio, news, and publications.

## Structure

- `_config.yml` — site-wide settings (title, author, social links, plugins).
- `_data/navigation.yml` — top menu.
- `_pages/about.md` — the homepage (bio + news).
- `_pages/publications.html` — the publications listing page.
- `_publications/` — one markdown file per paper.
- `_pages/Resume.pdf`, `_pages/MyResearch.pdf` — linked from the homepage.
- `images/` — avatar, favicons, and publication thumbnails.
- `_layouts/`, `_includes/`, `_sass/`, `assets/` — theme internals (rarely need editing).

## Adding a publication

Create a new file in `_publications/`, e.g. `_publications/my-paper.md`:

```yaml
---
title: "Paper title"
collection: publications
category: manuscripts
permalink: /publication/YYYY-MM-DD-short-slug
excerpt: "One-sentence summary."
venue: "Venue name"
year: 2026
paperurl: "https://arxiv.org/abs/xxxx.xxxxx"
image: "/images/publications/thumbnail.png"
---
```

Add the matching thumbnail under `images/publications/`.

## Running locally

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

Then open <http://localhost:4000>.

## Credits

Built with [Jekyll](https://jekyllrb.com) on the [Academic Pages](https://github.com/academicpages/academicpages.github.io) template, which is itself based on the [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) theme by Michael Rose. Licensed under the MIT License (see [`LICENSE`](LICENSE)).
