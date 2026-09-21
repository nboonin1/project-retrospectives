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

Pages, Discussions, and the giscus repo/category IDs in `_includes/comments.html` are already
configured. The one remaining step: install the [giscus GitHub App](https://github.com/apps/giscus)
on this repo (needs a browser + your GitHub login) so it's authorized to post comments as
Discussions. Without it, the comment widget loads but can't submit anything.
