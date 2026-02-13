# 🌐 elmaleek.me — Personal Site & Blog

This repository contains the source code for my personal website and blog:

👉 https://elmaleek.me

A simple, fast, and developer-focused site where I share what I’m building, learning, and experimenting with.

---

## ✨ About

This site serves as:

- Personal portfolio  
- Technical blog  
- Notes on things I build and learn  
- A place to share tutorials, tips, and thoughts  

Content is written in Markdown and built into a static site.

---

## 🛠 Tech Stack

- **Jekyll** — static site generator  
- **GitHub Pages** — hosting  
- **Markdown** — content writing  
- **HTML/CSS** — custom styling  
- **Liquid** — templating  

No database, no CMS, no heavy frameworks.

---

## 🚀 Local Development

### Install dependencies

```bash
bundle install
```

### Run locally

```bash
bundle exec jekyll serve --livereload
```

Open in browser:

```
http://127.0.0.1:4000
```

---

## ✍️ Writing a Post

Create a file inside:

```
_posts/
```

Filename format:

```
YYYY-MM-DD-title.md
```

Example:

```
2026-02-14-my-post.md
```

Basic front matter:

```md
---
layout: post
title: "My Post Title"
subtitle: "Optional subtitle"
tags: [dev, learning]
excerpt: "Short description for blog cards."
---
```

Then write your content in Markdown.

Push to the main branch and GitHub Pages will build automatically.

---

## 📁 Project Structure

```
_layouts/      → page layouts  
_posts/        → blog posts  
assets/        → images, CSS, files  
_config.yml    → site config  
index.md       → homepage  
about.md       → about page  
```

---

## 🎯 Goals

- Keep it simple  
- Fast loading  
- Easy to write content  
- Minimal maintenance  
- Focus on writing, not tooling  

---

## 📬 Contact

- Website: https://elmaleek.me  
- GitHub: https://github.com/elmaleek03  

---

## 📄 License

Open for learning and inspiration.  
Content is personal unless stated otherwise.
