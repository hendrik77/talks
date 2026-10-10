# Talks

Collection of presentation slides built with the help of AI. Most talks use [Slidev](https://sli.dev/), but other formats are welcome.

## Presentation formats

| Format | Source | How to view / build |
| --- | --- | --- |
| **Slidev** | `slides.md` + `package.json` | `npm install && npm run dev` (or `pnpm`) in the talk folder; `npm run build` / `npm run export` |
| **Marp** | Single Markdown file with `marp: true` frontmatter | Open the exported `.html` / `.pdf`, or rebuild with `npx @marp-team/marp-cli <deck>.md --html` (add `--pdf` for PDF) |
| **Images** | SVG / PNG slides | Open the image files directly in a browser or image viewer; no build step |

## Presentations

### [MCP'fication of SAP](./MCPficationOfSAP/)

How the Model Context Protocol (MCP) is transforming SAP development. Covers MCP basics, SAP TechEd 2025 announcements, official SAP MCP servers (CAP, Fiori, UI5, MDK), community-built servers, real-world use cases, and the outlook for the agentic enterprise.

*Format: Slidev*

### [SAP Stammtisch Frankfurt PLUS - Februar 2026](./SAPStammtischFRA-2026-02/)

Community slides for the 94th SAP Stammtisch Frankfurt, hosted at DZ BANK on February 11, 2026. Covers community updates, the move from Meetup to openMeet, the talk agenda, and evening dinner plans.

*Format: Slidev*

### [Decisions in Milliseconds: Jev & System One Models](./Jev_and_the_Rise_of_System_One_Models/)

AI Lunch talk (2 October 2026) on Jev and the rise of fast "System One" models. Includes the Marp deck (`ai-lunch-jev-system-one.md`) with HTML and PDF exports, a reading companion article, the underlying research document, and the live-demo code (`jev-demo.zip`).

*Format: Marp*

### [Agentic Engineering](./agentic_engineering/)

Image-only slides on agentic engineering: the five levels from prompting to orchestration, the four shifts towards loops, and a planner/generator/evaluator orchestration setup. A combined PDF (`bu-ai-lunch-agentic-engineering.pdf`) is included.

*Format: Images (SVG + PDF)*

## Licence

This work is licensed under [Creative Commons Attribution 4.0 (CC-BY-4.0)](./LICENCE.md).
