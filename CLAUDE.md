# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Slidev presentation project - a Vue 3 and Vite-powered slide deck framework for developers. The main presentation content lives in `slides.md`.

## Commands

```bash
pnpm install    # Install dependencies
pnpm dev        # Start dev server at localhost:3030
pnpm build      # Build for production (outputs to dist/)
pnpm export     # Export slides to PDF/PPTX/PNG
```

## Architecture

- **slides.md**: Main presentation file using Markdown with YAML frontmatter
- **components/**: Vue 3 components (script setup + TypeScript) usable directly in slides
- **snippets/**: TypeScript files with region markers (`// #region name`) for importing code into slides
- **pages/**: Additional slide fragments that can be imported via `src:` attribute

## Key Patterns

- Use pnpm (not npm) - configured with shamefully-hoist
- Vue 3 Composition API with `<script setup>` syntax
- UnoCSS utilities for styling (Tailwind-compatible classes)
- Code snippets use region markers: `<<< @/snippets/file.ts#regionName`
- Slidev supports MDC syntax, Mermaid diagrams, LaTeX, and Monaco editors
