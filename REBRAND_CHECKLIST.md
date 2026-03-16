# Rebrand Checklist: vibe-kanban → Kira Code

Use this checklist to track rebrand updates systematically.

## Phase 1: Critical Public-Facing Changes ⭐

### Root & Main Documentation
- [ ] `README.md` - Update all KairosUtamaIndonesia/kira-code URLs and package references (lines 4-6, 13, 14-15, 22, 42, 51, 64, 68)
- [ ] `package.json` - Line 2: Change `"name": "vibe-kanban"` → `"kira-code"`
- [ ] `package.json` - Line 6: Update CLI bin name if needed

### NPX CLI Package
- [ ] `npx-cli/package.json` - Line 2: Change `"name": "vibe-kanban"` → `"kira-code"`
- [ ] `npx-cli/package.json` - Line 7: Update bin mapping name
- [ ] `npx-cli/package.json` - Line 17: Update repository URL to new organization
- [ ] `npx-cli/package.json` - Line 23: Update description references
- [ ] `npx-cli/README.md` - Update all `npx vibe-kanban` examples (lines 10, 18-21, 179)

### Core Documentation
- [ ] `docs/index.mdx` - Line 14: Update installation command
- [ ] `docs/getting-started.mdx` - Update installation command
- [ ] `docs/cloud/getting-started.mdx` - Update installation command  
- [ ] `docs/troubleshooting.mdx` - Lines 27, 45, 51, 57, 60: Update paths and commands

---

## Phase 2: High-Priority API & Configuration

### GitHub Integration & API
- [ ] `crates/server/src/routes/releases.rs` - Line 14: Update GITHUB_API_URL
- [ ] `packages/web-core/src/shared/hooks/useGitHubStars.ts` - Line 6: Update API endpoint
- [ ] `packages/web-core/src/shared/dialogs/global/ReleaseNotesDialog.tsx` - Line 15: Update releases URL

### Frontend Links
- [ ] `packages/ui/src/components/AppBar.tsx` - Line 392: Update GitHub link href
- [ ] `packages/web-core/src/features/onboarding/ui/LandingPage.tsx` - Line 117: Update GitHub link

### Rust Backend
- [ ] `crates/tauri-app/Cargo.toml` - Lines 2, 7: Update package name `vibe-kanban-tauri` → `kira-code-tauri`
- [ ] `crates/remote/Cargo.toml` - Line 17: Update private repo dependency (coordinate with infrastructure team)

### Configuration & Documentation JSON
- [ ] `docs/docs.json` - Lines 138, 177: Update GitHub references
- [ ] `packages/local-web/vite.config.ts` - Line 111: Update Sentry project name

---

## Phase 3: Frontend Branding & Onboarding

### Logo Assets
- [ ] Create/rename logo files: `vibe-kanban-logo.svg` → `kira-code-logo.svg` and dark variant
- [ ] Update all references:
  - [ ] `packages/remote-web/src/shared/components/BrandLogo.tsx` - Lines 13, 16
  - [ ] `packages/web-core/src/pages/migrate/MigratePage.tsx` - Lines 49-50
  - [ ] `packages/web-core/src/features/onboarding/ui/OnboardingSignInPage.tsx` - Lines 99-100
  - [ ] `packages/web-core/src/features/onboarding/ui/LandingPage.tsx` - Lines 179-180
  - [ ] `README.md` - Logo image source tags

### Frontend Code
- [ ] `packages/web-core/src/shared/dialogs/command-bar/CreatePRDialog.tsx` - Line 51: Update PR title suffix
- [ ] `packages/web-core/src/pages/workspaces/PreviewBrowserContainer.tsx` - Line 675: Update source identifier
- [ ] `packages/web-core/src/shared/lib/relayPake.ts` - Lines 5-6: Update SPAKE2 IDs
- [ ] `packages/web-core/src/shared/actions/index.ts` - Line 859: Update comment
- [ ] `packages/web-core/src/shared/lib/diffDataAdapter.ts` - Lines 24, 73, 78: Update comments

---

## Phase 4: Documentation

### Workspace & Configuration Docs
- [ ] `docs/settings/general.mdx` - Line 149: Document new workspace directory path (`.kira-code-workspaces`)
- [ ] `docs/workspaces/creating-workspaces.mdx` - Update workspace directory references
- [ ] `docs/workspaces/managing-workspaces.mdx` - Update paths and examples
- [ ] `docs/workspaces/repositories.mdx` - Update workspace directory config

### Internationalization Files (i18n)
- [ ] `packages/web-core/src/i18n/locales/en/settings.json` - Lines 160, 163
- [ ] `packages/web-core/src/i18n/locales/zh-Hans/settings.json` - Lines 160, 163
- [ ] `packages/web-core/src/i18n/locales/zh-Hant/settings.json` - Lines 160, 163
- [ ] `packages/web-core/src/i18n/locales/es/settings.json` - Lines 160, 163
- [ ] `packages/web-core/src/i18n/locales/ja/settings.json` - Lines 160, 163
- [ ] `packages/web-core/src/i18n/locales/fr/settings.json` - Lines 160, 163
- [ ] `packages/web-core/src/i18n/locales/ko/settings.json` - Lines 160, 163

### Feature Documentation
- [ ] `docs/integrations/vibe-kanban-mcp-server.mdx` - Rename file and update all references
- [ ] `docs/integrations/mcp-server-configuration.mdx` - Update references
- [ ] `docs/core-features/testing-your-application.mdx` - Update `vibe-kanban-web-companion` package name
- [ ] `docs/core-features/creating-tasks.mdx` - Update references
- [ ] `docs/configuration-customisation/agent-configurations.mdx` - Update card title/reference

### Agent Integration Docs
- [ ] `docs/agents/amp.mdx` - Update `npx vibe-kanban` command
- [ ] `docs/agents/cursor-cli.mdx` - Update command
- [ ] `docs/agents/openai-codex.mdx` - Update command
- [ ] `docs/agents/claude-code.mdx` - Update command
- [ ] `docs/agents/droid.mdx` - Update command
- [ ] `docs/agents/gemini-cli.mdx` - Update command
- [ ] `docs/agents/qwen-code.mdx` - Update command
- [ ] `docs/agents/github-copilot.mdx` - Update command
- [ ] `docs/agents/opencode.mdx` - Update command

### Docker & Deployment Docs
- [ ] `docs/self-hosting/deploy-docker.mdx` - Lines 33, 34: Update git clone URL
- [ ] `docs/self-hosting/local-development.mdx` - Lines 20, 21: Update git clone URL
- [ ] `docs/cloud/index.mdx` - Update `npx vibe-kanban` commands
- [ ] `docs/cloud/troubleshooting.mdx` - Lines 296, 303: Update GitHub issue URLs

### VSCode Extension Docs
- [ ] `docs/integrations/vscode-extension.mdx` - Update marketplace links and extension ID (bloop.vibe-kanban → bloop.kira-code or similar)

### Other Docs
- [ ] `docs/cloud/projects.mdx` - Line 35: Update project abbreviation example ("VI" for vibe-kanban)
- [ ] `docs/README.md` - Check for any references
- [ ] All `.mdx` files - Global search for remaining references

---

## Phase 5: CLI & Build Infrastructure

### NPX CLI Code
- [ ] `npx-cli/src/cli.ts` - Lines 209-310: Update all CLI text, help messages, and command names
- [ ] `npx-cli/src/desktop.ts` - Line 238: Update command/label reference
- [ ] `npx-cli/src/download.ts` - Lines 10, 202: Update cache directory path (`.vibe-kanban` → `.kira-code`)

### Build Scripts
- [ ] `local-build.sh` - Update all binary names and references (lines 58-84)
- [ ] `.gitignore` - Lines 75-76, 85: Update patterns
- [ ] `scripts/generate-tauri-update-json.js` - Update comments and URL pattern

### Workflow Files (GitHub Actions)
- [ ] `.github/workflows/test.yml` - Lines 251, 304: Update crate exclusion name
- [ ] `.github/workflows/pre-release.yml` - Update all binary names and artifact references
- [ ] `.github/workflows/relay-deploy-dev.yml` - Line 22: Coordinate remote deployment repo rename
- [ ] `.github/workflows/relay-deploy-prod.yml` - Line 101: Coordinate remote deployment repo rename
- [ ] `.github/workflows/remote-deploy-dev.yml` - Line 23: Coordinate remote deployment repo rename
- [ ] `.github/workflows/remote-deploy-prod.yml` - Line 109: Coordinate remote deployment repo rename

---

## Phase 6: Test Data & Generated Files

### Mock Data (Optional - Only if user-facing)
- [ ] `packages/web-core/src/mock/normalized_entries.json` - May not need changes (test data paths)
- [ ] `packages/web-core/src/test/fixtures/normalized_entries.json` - May not need changes

### Test Fixtures
- [ ] `scripts/relay-test-client/index.html` - Line 224-225: Update SPAKE2 IDs
- [ ] `mobile-testing.md` - Line 139: Update example app name

### Auto-Generated Files (Skip - will auto-update)
- [ ] `Cargo.lock` - Will update with `cargo build`
- [ ] `npx-cli/package-lock.json` - Will update with `npm install`

---

## Phase 7: Verification & Testing

### Code Cleanup
- [ ] Run `pnpm run format` to format all code
- [ ] Run `pnpm run lint` to check for issues
- [ ] Run `pnpm run check` for TypeScript type checking

### Build & Test
- [ ] Test local build: `pnpm run dev`
- [ ] Build NPX CLI: `pnpm run build:npx`
- [ ] Test CLI: `npx kira-code --help`
- [ ] Verify backend builds: `pnpm run backend:check`

### Verification Checklist
- [ ] All GitHub URLs point to new repository
- [ ] All `npx vibe-kanban` commands updated to `npx kira-code`
- [ ] Logo assets renamed and referenced correctly
- [ ] i18n strings don't contain hardcoded "vibe-kanban" text
- [ ] Workspace directory configuration points to `.kira-code-workspaces`
- [ ] API endpoints (GitHub releases, stars) point to correct repository
- [ ] VSCode extension ID updated (if applicable)
- [ ] No broken documentation links
- [ ] Binary names reflect new branding

---

## Phase 8: Final Steps

### Repository Configuration
- [ ] Update GitHub repository name (if needed)
- [ ] Update repository description
- [ ] Update repository topics
- [ ] Update GitHub Pages settings

### Release & Publishing
- [ ] Tag new version in git
- [ ] Update CHANGELOG.md with rebrand notes
- [ ] Publish updated npm package `kira-code`
- [ ] Announce rebrand in release notes

### Post-Rebrand
- [ ] Monitor for broken links/references
- [ ] Update external documentation that references the old name
- [ ] Check for community mentions/issues about the rebrand
- [ ] Update social media and marketing materials

---

## Notes

### Searching for Remaining References
If you need to find any remaining references:
```bash
# Search for vibe-kanban references
grep -r "vibe-kanban" --include="*.ts" --include="*.tsx" --include="*.md" --include="*.mdx" --include="*.json" --include="*.toml"

# Search for BloopAI organization
grep -r "BloopAI" --include="*.ts" --include="*.tsx" --include="*.md" --include="*.mdx" --include="*.json" --include="*.toml"

# Search for bloop organization/branding
grep -r "bloop" --include="*.ts" --include="*.tsx" --include="*.md" --include="*.mdx" --include="*.json" --include="*.toml"
```

### Directory Path Changes
The `.vibe-kanban-workspaces` directory structure will need migration:
- New apps will use `.kira-code-workspaces`
- Consider migration script for existing user installations
- Update documentation on migration process

### External Dependencies
These repositories may need to be renamed/updated separately:
- `KairosUtamaIndonesia/kira-code-remote-deployment` - Coordinate with ops team
- `KairosUtamaIndonesia/kira-code-private` - Check Cargo.toml dependency
- VSCode extension repository (if separate)

