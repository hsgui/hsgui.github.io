# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal technical blog built with Jekyll, hosted on GitHub Pages at https://hsgui.github.io. Includes blog posts (Markdown) and two standalone developer tools (JSON to YAML converter, ClipGist for clipboard-to-Gist sharing).

## Commands

```bash
# Install dependencies
bundle install

# Run local development server (serves at http://localhost:4000)
bundle exec jekyll serve
```

## Architecture

**Jekyll Static Site** with standard structure:
- `_posts/` - Blog posts as Markdown files (naming: `YYYY-MM-DD-title.md`)
- `_layouts/` - Page templates (default → page/post inheritance)
- `_includes/` - Reusable HTML partials (header, footer, icons)
- `_sass/` - SCSS stylesheets, compiled via `css/main.scss`
- `_config.yml` - Site configuration

**Standalone Tool Pages** (no Jekyll processing, self-contained HTML/CSS/JS):
- `json2yaml.html` - JSON to YAML converter
- `clipgist.html` - Clipboard analyzer with GitHub Gist integration (uses localStorage for auth token)

**Deployment:** Automatic via GitHub Pages from master branch. No manual build step required.

## Creating New Posts

Add file to `_posts/` with front matter:
```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD HH:MM:SS +0800
categories: category1 category2
---
```
