# Kira Code Rebrand Plan

## Context

Rebranding from "Vibe Kanban" to "Kira Code" - comprehensive rebrand affecting packages, CLI, URLs, docs, env vars, and assets.

## Scope

- ~82 files, 450+ occurrences
- 10 categories: NPM, Rust, GitHub URLs, env vars, paths, assets, docs, frontend, i18n, build

## Key Changes

1. **NPM**: `vibe-kanban` → `kira-code`
2. **Rust**: `vibe-kanban-mcp`, `vibe-kanban-tauri` → `kira-code-mcp`, `kira-code-tauri`
3. **GitHub**: `KairosUtamaIndonesia/kira-code` → new org
4. **Env Vars**: `VK_*` → `KIRA_*`, `VITE_VK_*` → `VITE_KIRA_*`
5. **Paths**: `.vibe-kanban-workspaces` → `.kira-code-workspaces`
6. **Assets**: 5 logo files to rename
7. **Docs**: 36+ MDX files
8. **i18n**: 7 locale files

## Phases

1. Critical public-facing (package.json, README)
2. GitHub URLs & API
3. Environment variables
4. Assets & frontend
5. Documentation
6. i18n
7. Build infrastructure
8. Verification & release

## Decisions

- **GitHub org**: `KairosUtamaIndonesia`
- **Repository**: `KairosUtamaIndonesia/kira-code`
- **NPM**: `kira-code` (unscoped for now, can add scope later)
- **VSCode extension**: TBD - can update later when extension is set up
- **Sentry**: TBD - can update later when Sentry project is set up
- **Domains**: `kira-code.kairos-it.com` (new domain ready)
- **Workspace migration**: Breaking change - document in release notes
- **Logo assets**: Use `kira_logo.svg` from project root
- **Breaking changes**: Document in CHANGELOG with migration guide

## Asset Migration Plan

1. Copy `kira_logo.svg` to `packages/public/kira-code-logo.svg`
2. Create dark variant `packages/public/kira-code-logo-dark.svg`
3. Generate favicon variants from logo
4. Update all logo references in code
