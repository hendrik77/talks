# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Slidev presentation about integrating Model Context Protocol (MCP) with SAP systems.

## Commands

```bash
npm run dev      # Start dev server (localhost:3030)
npm run build    # Build for production
npm run export   # Export to PDF
```

## Structure

- `slides.md` - Main presentation file (Slidev markdown format)
- `package.json` - Dependencies and scripts

## Slidev Notes

- Slides separated by `---`
- First frontmatter block configures the deck
- Use `v-click` / `v-clicks` for animations
- Presenter notes go in HTML comments `<!-- -->`
- Mermaid diagrams supported in code blocks

## Version Control

Use **jj** (Jujutsu) for version control, not git. See https://docs.jj-vcs.dev/latest/

Common commands:
```bash
jj status          # Show working copy status
jj diff            # Show changes
jj new             # Create new change
jj describe -m ""  # Set change description
jj log             # Show revision history
jj git push        # Push to Git remote
```
