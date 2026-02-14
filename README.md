# samueljkeller.com – Personal Portfolio & Online Resume

![Website preview](https://raw.githubusercontent.com/samueljkeller/samueljkeller/main/static/images/preview.png)
<!-- ↑ Replace this with a real screenshot: save one in /static/preview.png and commit it -->

This is the complete source code for **samueljkeller.com** — my personal portfolio website and online resume.

It serves two main purposes:

1. **Professional showcase**  
   Demonstrates my skills in modern web development, static site generation, responsive design, CI/CD pipelines, and clean code practices. Potential employers and collaborators can review the code, architecture, and deployment workflow directly.

2. **Reusable template**  
   The repository is structured so anyone can easily fork it and turn it into their own personal portfolio or resume site with minimal effort.

Built with **Hugo** + **Tailwind CSS**, featuring light/dark mode, print-friendly styling, smooth animations, and fully automated deployment via **Azure Static Web Apps** + GitHub Actions.

## ✨ Features

- Clean, responsive one-page layout (mobile-first)
- Automatic light/dark mode (system preference + toggle)
- Tailwind CSS v3+ utility-first styling
- Hugo static site generation — extremely fast builds & live reload
- Markdown-driven content (easy updates to bio, projects, experience, etc.)
- Well-organized sections: Hero/About · Skills · Experience · Projects · Education · Contact
- SEO optimized (meta tags, Open Graph, Twitter Cards)
- Smooth scroll, subtle animations, and transitions
- Print-friendly resume view (Ctrl+P → Save as PDF)
- Full CI/CD pipeline with **Azure Static Web Apps** (free hosting, global CDN, custom domain, automatic SSL)

## 🌐 Live Site

**[https://samueljkeller.com](https://samueljkeller.com)**  
(Deployed via Azure Static Web Apps with custom domain)

## Why This Tech Stack?

This project reflects real-world choices I make as a developer:

- **Hugo** → lightning-fast builds, excellent content workflow via Markdown, no runtime overhead
- **Tailwind CSS** → rapid prototyping, consistent design system, built-in dark mode support
- **Azure Static Web Apps** → free tier, global edge caching, automatic HTTPS, integrated GitHub Actions CI/CD, custom domains — perfect for personal sites and JAMstack projects
- **Open source** → transparent code that hiring managers can audit

## 🚀 Quick Start (Using as Your Own Portfolio Template)

1. **Fork** this repository (recommended) or clone it directly
2. Rename it to something like `yourname-portfolio` or `yourname-resume`
3. Update `config.toml` with your name, bio, photo, social links, etc.
4. Replace or edit Markdown files in `/content/` (about.md, experience/, projects/, etc.)
5. (Optional) Adjust colors, fonts, or layout via Tailwind classes or custom CSS
6. Deploy — see Azure instructions below

### Prerequisites

- [Hugo](https://gohugo.io/installation/) (extended edition recommended)
- [Node.js](https://nodejs.org/) v18+ (only needed if you customize Tailwind styles)
- Git

### Local Development

```bash
# Clone your fork
git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
cd YOUR-REPO-NAME

# Install Tailwind (only if editing styles)
npm install

# Start dev server
hugo server --minify

# With drafts & future content visible:
# hugo server --minify --buildDrafts --buildFuture