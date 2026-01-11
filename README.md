# Shuigui & Learning

Personal technical blog built with Jekyll and hosted on GitHub Pages.

**Live Site:** [https://hsgui.github.io](https://hsgui.github.io)

## About

This is a personal blog for sharing learning notes on various programming and technology topics, including:

- Deep Learning & Machine Learning
- Reinforcement Learning
- C/C++ Programming
- Big Data
- Web Technologies (HTML, CSS, JavaScript)

## Tools

- **[JSON to YAML](/json2yaml.html)** - Convert JSON to YAML instantly
- **[ClipGist](/clipgist.html)** - Paste clipboard content and share to GitHub Gist with one click

## Tech Stack

- **Static Site Generator:** Jekyll
- **Hosting:** GitHub Pages
- **Styling:** Sass/SCSS
- **Markdown:** Kramdown

## Project Structure

```
.
├── _config.yml          # Site configuration
├── _includes/           # Reusable HTML partials (header, footer, etc.)
├── _layouts/            # Page templates (default, post, page)
├── _posts/              # Blog posts in Markdown
├── _sass/               # SCSS stylesheets
├── css/                 # Main stylesheet entry point
├── resume/              # LaTeX resume files
├── about.md             # About page
├── feed.xml             # RSS feed
├── Gemfile              # Ruby dependencies
└── index.html           # Homepage
```

## Local Development

### Prerequisites

- Ruby (2.0+)
- Bundler

### Setup

```bash
# Install dependencies
bundle install

# Run local server
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`.

## Creating New Posts

Add a new Markdown file in `_posts/` with the naming convention:

```
YYYY-MM-DD-title.md
```

Include front matter at the top:

```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD HH:MM:SS +0800
categories: category1 category2
---
```

## License

Content is personal and for educational purposes.

## Contact

- GitHub: [@hsgui](https://github.com/hsgui)
- Twitter: [@HShuigui](https://twitter.com/HShuigui)
