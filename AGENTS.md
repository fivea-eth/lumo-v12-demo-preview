# LUMO V12 Demo Preview Rules

## Purpose

This repository is a public, static preview artifact for the accepted LUMO V12 720p demo. It supports an English default and a complete Simplified Chinese browsing mode through `?lang=zh`. The private `lumo-interactive-demo` workspace remains the source of truth.

## Structure

- `/index.html`, `/404.html`: generated entry points.
- `/assets/`: generated CSS, JavaScript and fonts.
- `/media/`: approved preview media only.
- `/README.md`: scope and sharing notes.

## Delivery Rules

- Never hand-edit generated HTML, CSS, JavaScript or media in this repository.
- Rebuild from the private source repository with `npm run build:pages`, then replace the generated preview as one versioned release.
- Do not add source code, credentials, customer data, payment integrations, 4K media or production-commerce configuration.
- Develop on a task branch. Do not merge or push changes to `main` without explicit user authorization.
- GitHub Pages may publish only the explicitly accepted preview branch.

## Cleanup

- Remove superseded hashed assets during the next generated release.
- Do not retain temporary build directories, browser traces or local caches in Git.
