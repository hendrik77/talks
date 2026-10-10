# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Monorepo of presentations. Each subdirectory is a self-contained talk. Talks can use different presentation tools, so check which format a talk uses before editing or building it:

| Format | How to recognise it | Talks |
| --- | --- | --- |
| **Slidev** | `slides.md` + `package.json` with `@slidev/cli` | `MCPficationOfSAP/`, `SAPStammtischFRA-2026-02/` |
| **Marp** | Single `.md` deck with `marp: true` in the frontmatter, no `package.json` | `Jev_and_the_Rise_of_System_One_Models/` |
| **Images** | Only image files (SVG/PNG), no source markdown | `agentic_engineering/` |

Never convert a talk to a different tool unless asked. Default to Slidev for new talks unless the user picks another format.

When adding a talk, also add it to `README.md` with a short description and a `*Format: ...*` line.

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

## Slidev talks

### Commands

Each Slidev presentation has its own scripts. Run from the presentation subdirectory:

```bash
pnpm install        # Install deps (SAPStammtischFRA-2026-02 uses pnpm)
npm install         # Install deps (MCPficationOfSAP uses npm)
npm run dev         # Start dev server at localhost:3030
npm run build       # Build static SPA into ./dist
npm run export      # Export slides to PDF (needs playwright-chromium)
```

Root `package.json` has shared devDependencies: `prettier` with `prettier-plugin-slidev` and `playwright-chromium`.

### Architecture

- `slides.md` is the main entry point for each deck (Slidev markdown format)
- `pages/` - additional slide files imported via `src:` frontmatter
- `components/` - Vue SFCs auto-registered and usable directly in slides
- `snippets/` - code snippets importable into slides
- Images/assets live alongside `slides.md` in the presentation root

### Conventions

- Slides separated by `---`; first `---` block is YAML frontmatter for deck config
- Layouts set per slide via `layout:` frontmatter (e.g., `image-right`, `two-cols`, `section`, `statement`)
- `::right::` slot syntax for multi-column layouts
- `v-click` / `v-clicks` for step animations
- Presenter notes in HTML comments `<!-- -->`
- MDC (Markdown Components) enabled via `mdc: true`

### Deployment

Slidev presentations include config for both Netlify (`netlify.toml`) and Vercel (`vercel.json`) with SPA fallback routing.

## Marp talks

- The deck is a single Markdown file (e.g. `ai-lunch-jev-system-one.md`) with `marp: true`, `theme`, `paginate` and a custom `style:` block in the frontmatter. Styling lives in that `style:` block, not in separate CSS files.
- Slides are separated by `---`; per-slide layouts are CSS classes set via directives such as `<!-- _class: cards -->` or `<!-- _class: figure -->`, defined in the `style:` block. Speaker notes are plain HTML comments.
- Images may be embedded as base64 data URIs, so the `.md` can be very large. Read it in ranges (or grep for slide text) instead of loading the whole file.
- No `package.json`. Build with Marp CLI from the talk folder:

  ```bash
  npx @marp-team/marp-cli ai-lunch-jev-system-one.md --html -o ai-lunch-jev-system-one.html
  npx @marp-team/marp-cli ai-lunch-jev-system-one.md --pdf --allow-local-files -o ai-lunch-jev-system-one.pdf
  ```

- The exported `.html` and `.pdf` are committed. After changing the deck, regenerate them so they stay in sync.
- Supporting material (article, `research.md`, demo zip) sits next to the deck. Keep facts and source numbering consistent between them when editing.
- Slidev conventions (`layout:`, `v-click`, `::right::`, Vue components) do **not** apply here.

## Image-based talks

- Slides are standalone image files (currently SVG), one per slide, with no build step.
- Edit SVGs directly: text is in `<text>` elements. Keep the existing visual style (fonts, colours, layout grid) consistent across all slides of the talk.
- The talk's PDF (e.g. `bu-ai-lunch-agentic-engineering.pdf`) is built from the images. After changing an SVG, regenerate the PDF rather than introducing a slide framework.

## Formatting

Prettier is configured at root level with `prettier-plugin-slidev`, but only for `slides.md` and `pages/*.md`. Do not run the Slidev parser on Marp decks or other markdown. Markdownlint config (`.markdownlint.json`) disables many rules to accommodate Slidev's non-standard markdown.
