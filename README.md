# Responsabil

A cybersecurity education blog focused on making online safety accessible to everyone in Moldova and Romania. The project aims to demystify IT security by translating complex threats into practical advice and essential news that helps readers:

- Protect personal data and finances
- Recognize fraud attempts before it's too late
- Teach how to use technology responsibly

"Responsabil" means "responsible" in Romanian — the name reflects our core belief that an responsible user is a safe user. This is a non-commercial project driven by passion for technology and the desire to build digital resilience in our communities.

Built with [Hugo](https://gohugo.io/) + [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme, deployed on Cloudflare Pages at [responsabil.uncommercial.org](https://responsabil.uncommercial.org).

---

Un blog de educație cibernetică axat pe accesibilizarea siguranței online pentru toți cetățenii din Moldova și România. Proiectul își propune să demitizeze securitatea IT prin traducerea amenințărilor complexe în sfaturi practice și știri esențiale care ajută cititorii să:

- Protejeze datele personale și economiile
- Recunoască tentativele de fraudă la timp
- Învețe cum să utilizeze tehnologia responsabil

„Responsabil" este numele nostru și promisiunea noastră — un utilizator informat este un utilizator în siguranță. Acesta este un proiect non-comercial, animat de pasiunea pentru tehnologie și de dorința de a construi reziliență digitală în comunitățile noastre.

---

## Contributing

We welcome contributions! To suggest changes or add new content:

1. **Fork the repository** on GitHub
2. **Create a new branch** for your feature or fix (`git checkout -b my-feature`)
3. **Make your changes** (edit posts, fix typos, improve documentation)
4. **Push to your fork** (`git push origin my-feature`)
5. **Open a Pull Request** against the `main` branch

### What you can contribute:
- New articles on cybersecurity topics
- Corrections or improvements to existing posts
- Translation improvements
- Documentation fixes

## Requirements

- [Hugo](https://gohugo.io/installation/) v0.157.0 extended (`brew install hugo`)
- [Go](https://go.dev/) 1.18+ (`brew install go`) — required for Hugo modules

## Local Development

Start the dev server with drafts enabled:

```bash
hugo server -D
```

Open [http://localhost:1313](http://localhost:1313) in your browser. The server hot-reloads on file changes.

Useful flags:

```bash
hugo server -D              # include draft posts
hugo server -D --disableFastRender  # full re-render on each change (slower but accurate)
hugo server --port 1314     # use a different port
```

## Build

Generate the static site into the `public/` directory:

```bash
hugo --minify
```

The `public/` folder is git-ignored — Cloudflare Pages builds it automatically on each push to `main`.

## Writing New Posts

### Create a post

```bash
hugo new content posts/CATEGORY/SUBCATEGORY/post-slug.md
```

Examples:

```bash
hugo new content posts/technology/web-development/my-post.md
hugo new content posts/lifestyle/weekend-trip.md
```

This uses the archetype at `archetypes/posts.md` and pre-fills the front matter.

### Front matter reference

```yaml
---
title: "Post Title"
date: 2026-03-04
draft: true          # set to false to publish
description: "Short summary shown in listings and SEO meta."
categories: ["tehnologie"]
tags: ["web", "hugo"]
cover:
  image: "cover.jpg" # place image in the same folder as the post
  alt: "Image description"
  caption: "Optional caption"
  relative: true
showToc: true        # show table of contents
---
```

### Drafts

Posts with `draft: true` are **not published**. To preview drafts locally:

```bash
hugo server -D
```

To publish a draft, set `draft: false`.

### Content sections (categories & subcategories)

Posts are organised using folder structure — this automatically generates listing pages:

```
content/posts/
  technology/               → /posts/technology/
    web-development/        → /posts/technology/web-development/
      my-post.md            → /posts/technology/web-development/my-post/
  lifestyle/                → /posts/lifestyle/
    my-post.md              → /posts/lifestyle/my-post/
```

To add a new category or subcategory, create a folder and an `_index.md` inside it:

```bash
mkdir -p content/posts/finance
cat > content/posts/finance/_index.md << 'EOF'
---
title: "Finanțe"
description: "Articole despre finanțe personale"
---
EOF
```

### Static pages (About, Privacy Policy, etc.)

Static pages live in `content/pages/`. Edit them directly:

- `content/pages/about.md`
- `content/pages/privacy-policy.md`

To add a new static page:

```bash
hugo new content pages/new-page.md
```

Then add it to the menu in `hugo.toml` if needed:

```toml
[[menus.main]]
  identifier = "new-page"
  name = "New Page"
  url = "/pages/new-page/"
  weight = 45
```

## Project Structure

```
.
├── archetypes/
│   └── posts.md          # template for new posts
├── content/
│   ├── posts/            # blog posts (organised by section/subsection)
│   ├── pages/            # static pages (about, privacy policy, etc.)
│   └── search.md         # search page
├── static/
│   ├── admin/            # Decap CMS files
│   └── images/           # media assets
├── themes/               # empty — PaperMod loaded via Hugo modules
├── go.mod                # Hugo module dependencies
├── go.sum
└── hugo.toml             # site configuration
```

## Updating the Theme

```bash
hugo mod get -u github.com/adityatelange/hugo-PaperMod
hugo mod tidy
```

## Decap CMS (Admin)

**Note**: Decap CMS will be run only locally.

The blog includes [Decap CMS](https://decapcms.org/) for visual content management. Access it at:

```
http://localhost:1313/admin/
```

### Managing Content

- **Posts**: Create new posts, edit existing ones, manage categories and tags
- **Pages**: Edit the About and Privacy Policy pages



