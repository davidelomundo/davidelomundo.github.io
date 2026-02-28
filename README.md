# Personal Portfolio Website

A modern, Apple-inspired personal portfolio website built with Hugo static site generator. Features a clean design with sections for Home, Projects, Journal, About, and Contact with white and dark mode themes and a responsive layout.

## 🚀 Quick Start

### Requirements

- <a href="https://gohugo.io/installation/" target="_blank" rel="noopener noreferrer">Hugo</a>

### Local Development

```bash
# Start Hugo development server
hugo server --buildDrafts

# Build for production
hugo --gc --minify
```

- Local server: `http://localhost:1313`

### Deploy to GitHub Pages

The site automatically deploys to GitHub Pages through GitHub Actions workflow defined in `.github/workflows/hugo.yml`.

## 📁 Project Structure

| Folder | Purpose |
|--------|---------|
| `assets/css/` | Stylesheets and design variables |
| `content/` | Markdown content (pages & journal posts) |
| `data/` | Data files (`projects.yaml`) |
| `layouts/` | Hugo templates and partials |
| `static/` | Images, resume, and other static assets |

## 🔧 Customization

### Update Content

1. **Projects**: Edit `/data/projects.yaml` to add/update projects
2. **Journal Posts**: Add markdown files to `/content/journal/`
3. **About Page**: Modify `/layouts/_default/about.html`
4. **Contact Info**: Update `/layouts/_default/contact.html`

## 📝 Adding Journal Posts

Create a new markdown file in `/content/journal/`:

```markdown
---
title: "Your Post Title"
date: 2026-02-27
draft: false
category: "Blog"
image: "/images/your-image.jpg"
excerpt: "A brief description of your post"
---

Your content here...
```