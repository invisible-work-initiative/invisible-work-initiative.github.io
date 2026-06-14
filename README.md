# Invisible Work Initiative — Website

This repository is the public website for the [Invisible Work Initiative](https://github.com/invisible-work-initiative), published with GitHub Pages at:

**https://invisible-work-initiative.github.io**

## How it works

The site uses GitHub Pages' built-in Jekyll with the `minima` theme. There is no build step to run locally. Push markdown to `main` and GitHub rebuilds the site automatically (usually within a minute or two).

- `index.md` — homepage
- `syllabus-ai-for-oss.md` — the M.Eng. project syllabus, published at `/ai-for-oss/`
- `_config.yml` — site title, description, theme, and header navigation

## Editing

Edit the markdown files directly. To add a new page (for example, a per-track page), create `trackname.md` with front matter like:

```yaml
---
layout: page
title: Track 1
permalink: /track-1/
---
```

Add the filename to `header_pages` in `_config.yml` if it should appear in the site header.

## License

Site text content is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). See `LICENSE.md`.
