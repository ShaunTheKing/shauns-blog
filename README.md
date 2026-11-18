# Shaun's Blog

A Jekyll blog hosted on GitHub Pages: https://shauntheking.github.io/shauns-blog/

## Writing a post

Add a Markdown file to `_posts/` named `YYYY-MM-DD-title.md` with front matter:

```markdown
---
layout: post
title: "My post title"
date: 2026-11-17 12:00:00 +0000
---

Post content here.
```

Push to `main` and GitHub Pages rebuilds the site automatically.

## Editing the site

- `_config.yml`: site title, description, links
- `about.md`: the About page
- Design: custom layouts in `_layouts/` and styles in `assets/css/style.css`

## Weekly AI News

Issues live at `/ai-news/`. To publish one:

1. Copy `_drafts/weekly-ai-news-template.md` into `_posts/` as `YYYY-MM-DD-weekly-ai-news.md`.
2. Fill it in. Keep `categories: ai-news` in the front matter so it shows up in the AI News section and gets the badge.
3. Push to `main`.

Files in `_drafts/` are never published.
