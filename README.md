
# 🖋️ Contributing to **AIGC Watermarking Blog**

This project is a static Jekyll + Chirpy site hosted on **GitHub Pages**. Every article is just a Markdown file committed to the repository.
We use a *plain* Git workflow—**submit a Pull Request, get it reviewed, merge, publish**—so no extra CMS or build server is required.

## 🏃‍♂️ Quick Start

1. **Fork** this repository to your own account (click the *Fork* button top‑right on GitHub).
2. **Clone** your fork locally:

   ```bash
   git clone https://github.com/<your‑username>/aigcwatermarking.github.io.git
   cd aigcwatermarking.github.io
   ```
3. **Create a post** (see below for naming and template).
4. **Commit & push** to a new branch on your fork.
5. **Open a Pull Request** targeting `main` on this repo.
6. A maintainer will review, request changes if needed, and merge. GitHub Pages will rebuild automatically.

> **Tip – GitHub Web Editor**: If you prefer, click *Add file → Create new file* in your fork to create the post directly in the browser, then open the PR. No local Git needed.



## 📄 File‑Name & Location

```
_posts/YYYY-MM-DD-your-title.md
```

* **Date** `YYYY-MM-DD` should match the intended publication day.
* **Slug** `your-title` should be lowercase, words separated by hyphens.

Images go under `assets/img/…` (create sub‑folders if you like).



## ✨ Post Front‑Matter Template

Paste the block below at the top of your new file and fill in each field.

```yaml
---
layout:   post
title:    "Concise, Descriptive Title"
author:   "Your Name"          # Optional—omit to hide
date:     2025-mm-dd            # ISO format
categories: [Image Watermarking]     # One or more high‑level buckets
tags:       [Diffusion, Robustness]  # Fine‑grained keywords
series:     "Deep Dive #1"          # Optional—link multi‑part series
summary: |
  Short abstract (1–3 sentences) shown on the home page.
keywords: [AIGC, Watermarking, Provenance]  # Optional, for SEO
comments: true      # true ➜ enable Utterances/Disqus; false ➜ hide
cover:    /assets/img/covers/your-image.png  # Optional teaser image
---
```

Start the body right after the closing `---`.

### Body Guidelines

* Use Markdown headings starting with `##` (the title is automatically `#`).
* Mathematical formulas (`$$`), code blocks <code>\`\`\`</code>, and Mermaid diagrams are supported out of the box.
* Insert figures with captions and reference them in the text.
* Cite sources with plain links or footnotes `[^1]`.
* End with an optional **Further Reading** or **Acknowledgements** section.


## 🔍 Local Preview (optional)

If you want to test the post locally before pushing:

```bash
bundle install          # first time only – installs Jekyll & deps
bundle exec jekyll s    # builds site and serves at http://127.0.0.1:4000
```

The Chirpy theme will hot‑reload on file changes.


## ✅ Commit Style & PR Checklist

* Write clear commit messages ("Add post: *Transformer Watermarks*" rather than "Update").
* Spell‑check and run Markdown lint if you have it.
* Ensure images are reasonably compressed (PNG/JPEG ≤ 1 MB if possible).
* Confirm the post renders correctly in the local preview or in the *Files changed* diff view.
