# 🔗 Technical Writing Links

[![Gem Version](https://img.shields.io/gem/v/jekyll.svg?color=red&label=Jekyll&logo=jekyll)][ruby-gems]
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](http://creativecommons.org/licenses/by/4.0/)
[![Deploy to GitHub Pages](https://github.com/zapata131/tw-links/actions/workflows/deploy.yml/badge.svg)](https://github.com/zapata131/tw-links/actions/workflows/deploy.yml)
[![Check Links](https://github.com/zapata131/tw-links/actions/workflows/links.yml/badge.svg)](https://github.com/zapata131/tw-links/actions/workflows/links.yml)

A curated collection of essential resources for technical writers. Visit the
live site at [technicalwriting.link][tw-link].

---

## Overview

This repository contains the source code for
[Technical Writing Links][tw-link], a simple and useful landing page for
documentation professionals. It's built with [Jekyll][jekyll] and the
[Biscuit][biscuit] theme, and GitHub Actions deploys it to GitHub Pages.

## Project structure

```text
.
├── twlinks/                  # Base folder with the Jekyll site
│   ├── _config.yml           # Main configuration file
│   ├── index.md              # Homepage content (the list of resources)
│   ├── about.md              # About page content
│   ├── _includes/            # HTML partials
│   │   └── icon.html         # Inline SVG icons for the section headings
│   ├── _layouts/             # Page layout
│   ├── _sass/                # SCSS partials (theme styles)
│   └── css/                  # SCSS entry point, compiled to css/main.css
└── .github/workflows/
    ├── deploy.yml            # Builds and deploys the site to GitHub Pages
    └── links.yml             # Checks every link with lychee
```

---

## Prerequisites and setup

To build and test this project locally, you need a stable Ruby environment.

### 1. Requirements

- **Ruby**: Version 3.1 or higher is recommended.
- **Bundler**: For managing project dependencies.
- **Git**: For version control.

### 2. Platform-specific installation

- **macOS**:
  ```bash
  brew install ruby
  gem install bundler
  ```
- **Linux (Ubuntu or Debian)**:
  ```bash
  sudo apt update
  sudo apt install ruby-full build-essential
  gem install bundler
  ```

### 3. Local installation

Navigate to the project subdirectory and install gems:

```bash
cd twlinks
bundle install
```

> [!TIP]
> **Linux users**: If you encounter platform errors, run:
> `bundle lock --add-platform x86_64-linux`

---

## Development workflow

### Preview locally

Start the Jekyll development server with live reloading:

```bash
bundle exec jekyll serve
```

The site is available at `http://localhost:4000`.

### Build for production

Generate the static assets in the `_site` directory:

```bash
bundle exec jekyll build
```

---

## Edit the content

### Add a resource

All the resources live in `twlinks/index.md`. To add one:

1. Find the section where the resource belongs.
2. Place the entry where it fits the section's progression (for example, from
   foundational to advanced, or from general to specialized), using this format:

   ```markdown
   - [Name of the resource](https://example.com/): A short description of
     what it is and why it's useful.
   ```

3. Open the link and confirm that it leads to the page you describe. A link
   can work and still point to the wrong thing, especially video links.

### Section icons

Each section heading starts with a small inline SVG icon instead of an emoji.
The icons come from [Lucide](https://lucide.dev) (ISC license) and are defined
in `twlinks/_includes/icon.html`. A heading looks like this:

```markdown
## {% include icon.html name="guides" %} Guides & Case Studies {#guides}
```

The available names are `guides`, `tools`, `courses`, `books`, `blogs`,
`podcasts`, `videos`, and `communities`. Keep an explicit `{#id}` anchor on
each heading so the top jump-link bar stays linked properly.

To add an icon for a new section, copy the shapes from the Lucide icon's SVG
into a new `when` branch in the `icon.html` file. Keep each branch on a single
line, because the output sits inside a Markdown heading.

---

## Link checking

The **Check Links** workflow (`.github/workflows/links.yml`) uses
[lychee](https://lychee.cli.rs) to check every link in the Markdown files
under `twlinks/`. It runs in these cases:

- On pushes to `main` and on pull requests that change those files.
- On the first day of every month, to catch links that stopped working.
- Manually, from the **Actions** tab.

A broken link makes the workflow fail. Keep these details in mind:

- `merriam-webster.com` and `academia.edu` are excluded, because they reject
  automated requests.
- Root-relative links, such as `/about.html`, are checked against the live
  site, so a link to a page that isn't deployed yet fails until it is.

---

## Collaboration practices

Contributions are welcome! To keep the quality high, follow these guidelines.

### Branching strategy

- **main**: The stable, production-ready branch. Don't commit major changes
  directly here.
- **feature/your-feature**: Create a branch for your specific task or resource
  addition.

### Contribution steps

1. **Fork** the repository.
2. **Create a branch** for your specific change.
3. **Commit** your changes with descriptive messages. For example,
   `feat: add link to The Good Docs Project`.
4. **Push** to your fork and submit a **Pull Request**.

### Quality checks

- Place new links in a logical spot within their section (for example, from
  foundational to advanced).
- Test your changes locally with `bundle exec jekyll serve` before you push.
- Make sure the **Check Links** workflow passes on your pull request.

---

## Deployment

### Automated (recommended)

Pushes to the `main` branch that change files in `twlinks/` or the
`.github/workflows/deploy.yml` file trigger the **Deploy to GitHub Pages**
workflow, which builds the site and deploys it to GitHub Pages.

### Manual

You can also start a deployment from the **Actions** tab in GitHub: select
the **Deploy to GitHub Pages** workflow, and then run it.

---

## Collaborators

Special thanks to the following people for their contributions and support:

- Ariel Sánchez, Aarón Martínez, and José Antonio Sánchez.
- **Meeta Gupta** for her invaluable mentorship.

---

[ruby-gems]: https://rubygems.org/gems/jekyll
[tw-link]: https://technicalwriting.link
[jekyll]: http://jekyllrb.com/
[biscuit]: http://sblisesivdin.github.io/biscuit
