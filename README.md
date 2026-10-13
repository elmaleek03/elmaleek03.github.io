# elmaleek.me

Source for my personal site and blog: https://elmaleek.me

A static site for writing about what I build, learn, and tinker with.

## Stack

- Jekyll (static site generator)
- GitHub Pages (hosting)
- Markdown (content), Liquid (templating)
- Handwritten HTML/CSS, no frameworks or JavaScript

## Local development

Install dependencies:

```bash
bundle install
```

Run the dev server:

```bash
bundle exec jekyll serve
```

Then open http://127.0.0.1:4000.

## Writing a post

Add a Markdown file to `_posts/` named `YYYY-MM-DD-title.md`:

```md
---
layout: post
title: "My Post Title"
subtitle: "Optional subtitle"
tags: [dev, learning]
excerpt: "Short description shown in the post list."
---

Post content in Markdown.
```

Push to `master` and GitHub Pages rebuilds automatically.

## Structure

```
_layouts/     page layouts
_includes/    reusable fragments
_posts/       blog posts
assets/       CSS, images, files
_config.yml   site config
index.md      homepage
about.md      about page
blog.md       blog index
```

## License

Personal content unless stated otherwise. Code is open for reference.
