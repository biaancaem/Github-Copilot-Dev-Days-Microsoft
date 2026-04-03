# Mona Mayhem: Copilot Instructions

## Project Overview
This repository is an Astro 5 app called Mona Mayhem.

Purpose:
- Build a small web app that compares GitHub contribution activity.
- Serve a web UI from `src/pages/index.astro`.
- Expose an API endpoint at `src/pages/api/contributions/[username].ts`.

Scope:
- Focus on the application in `src/`, `public/`, and root Astro config files.
- Ignore all content in `workshop/` unless explicitly asked.

## Build and Dev Commands
Run all commands from the repository root.

- Install dependencies: `npm install`
- Start dev server: `npm run dev`
- Build production output: `npm run build`
- Preview production build: `npm run preview`
- Astro CLI (direct): `npm run astro -- <command>`

## Astro Best Practices
- Keep page routes in `src/pages/`; file-based routing is the source of truth.
- Use `.astro` components for page markup and composition.
- Keep server-only logic in API routes (for example, `src/pages/api/**`).
- Return explicit status codes and JSON headers from API handlers.
- Validate route params and fail fast with clear error responses.
- Avoid hardcoding secrets; use environment variables for tokens and keys.
- Keep styles organized and reuse shared CSS where practical.
- Prefer small, composable components over large monolithic pages.
- Keep TypeScript types explicit in API handlers (`APIRoute`) and shared utilities.
- If adding SSR behavior, keep `prerender` settings intentional and documented.

## Implementation Notes for This Repo
- `astro.config.mjs` is configured for server output with the Node adapter in standalone mode.
- The contributions endpoint is currently a scaffold and expected to be implemented.
- Keep changes minimal, readable, and aligned with existing style in this repository.
