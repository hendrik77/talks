# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Monorepo of Slidev presentations. Each subdirectory is a self-contained talk with its own `package.json`, `slides.md`, and assets.

## Version Control

Use **jj** (Jujutsu) for version control, not git. Never use `git commit`, `git add`, or other git mutation commands. The repo is colocated (`.jj/` + `.git/`).

```bash
jj status          # Show working copy status
jj diff            # Show changes
jj new             # Create new change
jj describe -m ""  # Set change description
jj log             # Show revision history
jj git push        # Push to Git remote
```

## Commands

Each presentation has its own scripts. Run from the presentation subdirectory:

```bash
pnpm install        # Install deps (SAPStammtischFRA-2026-02 uses pnpm)
npm install         # Install deps (MCPficationOfSAP uses npm)
npm run dev         # Start dev server at localhost:3030
npm run build       # Build static SPA into ./dist
npm run export      # Export slides to PDF (needs playwright-chromium)
```

Root `package.json` has shared devDependencies: `prettier` with `prettier-plugin-slidev` and `playwright-chromium`.

## Architecture

- **One directory per talk** (e.g., `MCPficationOfSAP/`, `SAPStammtischFRA-2026-02/`)
- `slides.md` is the main entry point for each deck (Slidev markdown format)
- `pages/` - additional slide files imported via `src:` frontmatter
- `components/` - Vue SFCs auto-registered and usable directly in slides
- `snippets/` - code snippets importable into slides
- Images/assets live alongside `slides.md` in the presentation root

## Slidev Conventions

- Slides separated by `---`; first `---` block is YAML frontmatter for deck config
- Layouts set per slide via `layout:` frontmatter (e.g., `image-right`, `two-cols`, `section`, `statement`)
- `::right::` slot syntax for multi-column layouts
- `v-click` / `v-clicks` for step animations
- Presenter notes in HTML comments `<!-- -->`
- MDC (Markdown Components) enabled via `mdc: true`

## Formatting

Prettier is configured at root level with `prettier-plugin-slidev` to handle `slides.md` and `pages/*.md` files. Markdownlint config (`.markdownlint.json`) disables many rules to accommodate Slidev's non-standard markdown.

## Deployment

Presentations include config for both Netlify (`netlify.toml`) and Vercel (`vercel.json`) with SPA fallback routing.
