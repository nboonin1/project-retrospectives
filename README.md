# project-retrospectives

Personal blog for project retrospectives — what worked, what didn't, what I'd do differently.
Built with Jekyll, hosted on GitHub Pages, comments via giscus.

## Writing a post

Add a file to `_posts/` named `YYYY-MM-DD-title.md`:

```markdown
---
layout: post
title: "Title"
date: YYYY-MM-DD
---

Body in markdown. Images go in assets/images/ and are referenced as /assets/images/name.png.
For video, embed a YouTube/Vimeo link rather than committing video files (see _posts/2026-09-21-welcome.md).
```

Push to `main` and GitHub Pages rebuilds automatically.

## Local preview (optional)

Requires Ruby + Bundler.

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## One-time setup after the repo exists on GitHub

1. **Enable Pages**: Settings → Pages → Source: Deploy from branch → `main` / `/ (root)`.
2. **Enable Discussions**: Settings → General → Features → check "Discussions".
3. **Install giscus**: go to [giscus.app](https://giscus.app), enter this repo, pick the "General"
   discussion category, and copy the `data-repo-id` and `data-category-id` values it generates
   into `_includes/comments.html` (replacing the `REPLACE_*` placeholders), along with the
   `data-repo` value (`owner/repo`).
