# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed

- **BREAKING CHANGE**: Complete rebrand from "Vibe Kanban" to "Kira Code"
  - NPM package renamed from `vibe-kanban` to `kira-code`
  - CLI command changed from `npx vibe-kanban` to `npx kira-code`
  - GitHub repository moved from `BloopAI/vibe-kanban` to `KairosUtamaIndonesia/kira-code`
  - Domain changed from `vibekanban.com` to `kira-code.kairos-it.com`
  - Environment variables renamed from `VK_*` prefix to `KIRA_*` prefix
  - Workspace directory changed from `.vibe-kanban-workspaces` to `.kira-code-workspaces`
  - Rust binaries renamed: `vibe-kanban-mcp` → `kira-code-mcp`, `vibe-kanban-tauri` → `kira-code-tauri`
  - All documentation, i18n, and frontend references updated

### Migration Guide

To migrate from Vibe Kanban to Kira Code:

1. **Update your CLI command**:
   ```bash
   # Old
   npx vibe-kanban
   
   # New
   npx kira-code
   ```

2. **Update environment variables** (if you had custom `.env` files):
   - `VK_ALLOWED_ORIGINS` → `KIRA_ALLOWED_ORIGINS`
   - `VK_SHARED_API_BASE` → `KIRA_SHARED_API_BASE`
   - `VK_SHARED_RELAY_API_BASE` → `KIRA_SHARED_RELAY_API_BASE`
   - `VK_TUNNEL` → `KIRA_TUNNEL`

3. **Workspace directories**: Existing workspaces in `.vibe-kanban-workspaces` will need to be moved to `.kira-code-workspaces` or re-created.

4. **Configuration files**: Update any custom configuration files that reference the old paths or names.

## [0.1.30] - 2025-03-16

### Added
- Initial release as Vibe Kanban
