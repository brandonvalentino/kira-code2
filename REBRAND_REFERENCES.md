# Rebrand References: KairosUtamaIndonesia/kira-code → Kira Code

Comprehensive list of all files containing references to "KairosUtamaIndonesia/kira-code", "github.com/KairosUtamaIndonesia/kira-code", and related vibe-kanban identifiers that need to be updated for the Kira Code rebrand.

---

## 1. Direct GitHub Repository References (KairosUtamaIndonesia/kira-code URLs)

These files contain explicit GitHub organization/repository references:

### 1.1 Package Configuration Files
- **`npx-cli/package.json`** (line 17)
  - Repository URL: `"url": "https://github.com/KairosUtamaIndonesia/kira-code"`
  
### 1.2 Documentation Files
- **`README.md`** (4 references)
  - Line 14: Build status badge URL
  - Line 15: DeepWiki badge URL  
  - Line 64: GitHub Discussions link
  - Line 68: GitHub Discussions link
  
- **`docs/self-hosting/local-development.mdx`** (1 reference)
  - Line 20: `git clone https://github.com/KairosUtamaIndonesia/kira-code.git`
  
- **`docs/self-hosting/deploy-docker.mdx`** (1 reference)
  - Line 33: `git clone https://github.com/KairosUtamaIndonesia/kira-code.git`
  
- **`docs/cloud/troubleshooting.mdx`** (2 references)
  - Line 296: GitHub issues link
  - Line 303: Report issue card href

### 1.3 TypeScript/React Code Files
- **`packages/ui/src/components/AppBar.tsx`** (1 reference)
  - Line 392: GitHub link in href attribute
  
- **`packages/web-core/src/features/onboarding/ui/LandingPage.tsx`** (1 reference)
  - Line 117: href to GitHub repository
  
- **`packages/web-core/src/shared/dialogs/global/ReleaseNotesDialog.tsx`** (1 reference)
  - Line 15: `const GITHUB_RELEASES_URL = 'https://github.com/KairosUtamaIndonesia/kira-code/releases'`
  
- **`packages/web-core/src/shared/hooks/useGitHubStars.ts`** (1 reference)
  - Line 6: GitHub API URL pointing to KairosUtamaIndonesia/kira-code repo

### 1.4 Rust Backend Code
- **`crates/server/src/routes/releases.rs`** (1 reference)
  - Line 14: `const GITHUB_API_URL: &str = "https://api.github.com/repos/KairosUtamaIndonesia/kira-code/releases"`
  
- **`crates/remote/Cargo.toml`** (1 reference)
  - Line 17: Git dependency on `ssh://git@github.com/KairosUtamaIndonesia/kira-code-private`

### 1.5 Configuration & Documentation JSON
- **`docs/docs.json`** (2 references)
  - Line 138: href to GitHub
  - Line 177: github field value

### 1.6 GitHub Workflows (Deployment)
- **`.github/workflows/relay-deploy-dev.yml`** (1 reference)
  - Line 22: `repository: KairosUtamaIndonesia/kira-code-remote-deployment`
  
- **`.github/workflows/relay-deploy-prod.yml`** (1 reference)
  - Line 101: `repository: KairosUtamaIndonesia/kira-code-remote-deployment`
  
- **`.github/workflows/remote-deploy-dev.yml`** (1 reference)
  - Line 23: `repository: KairosUtamaIndonesia/kira-code-remote-deployment`
  
- **`.github/workflows/remote-deploy-prod.yml`** (1 reference)
  - Line 109: `repository: KairosUtamaIndonesia/kira-code-remote-deployment`

### 1.7 Build & Script Files
- **`scripts/generate-tauri-update-json.js`** (1 reference)
  - Line 10: Commented URL with KairosUtamaIndonesia/kira-code

---

## 2. Indirect References (vibe-kanban package names, identifiers, workspace directories, etc.)

These files reference "vibe-kanban" as package names, binaries, directories, or identifiers that are tied to the project:

### 2.1 Root Configuration Files
- **`package.json`** (2 references)
  - Line 2: `"name": "vibe-kanban"`
  - Line 6: CLI bin name: `"vibe-kanban": "npx-cli/bin/cli.js"`
  
- **`.gitignore`** (3 references)
  - Line 75: `npx-cli/vibe-kanban-*`
  - Line 76: `vibe-kanban-*.tgz`
  - Line 85: `vibe-kanban-cloud/`

### 2.2 NPX CLI Package
- **`npx-cli/package.json`** (3 references)
  - Line 2: `"name": "vibe-kanban"`
  - Line 7: `"vibe-kanban": "bin/cli.js"`
  - Line 23: Package description references vibe-kanban
  
- **`npx-cli/package-lock.json`** (2 references)
  - Line 2: package name
  - Line 8: package name in dependencies
  
- **`npx-cli/README.md`** (7 references)
  - Lines 10, 18-21, 179: `npx vibe-kanban` commands in documentation
  
- **`npx-cli/src/cli.ts`** (6 references)
  - Lines 209, 217, 234, 255, 276, 310, 313: CLI references and help text
  
- **`npx-cli/src/desktop.ts`** (1 reference)
  - Line 238: Reference in command/label
  
- **`npx-cli/src/download.ts`** (2 references)
  - Line 10: Cache directory `.vibe-kanban`
  - Line 202: Path reference

### 2.3 Frontend Web App Files
- **`packages/local-web/vite.config.ts`** (1 reference)
  - Line 111: Sentry configuration `project: 'vibe-kanban'`
  
- **`packages/remote-web/src/shared/components/BrandLogo.tsx`** (2 references)
  - Lines 13, 16: Logo file references `/vibe-kanban-logo-*`
  
- **`packages/web-core/src/pages/migrate/MigratePage.tsx`** (2 references)
  - Lines 49-50: Logo asset references
  
- **`packages/web-core/src/features/onboarding/ui/OnboardingSignInPage.tsx`** (2 references)
  - Lines 99-100: Logo asset references
  
- **`packages/web-core/src/features/onboarding/ui/LandingPage.tsx`** (2 references)
  - Lines 179-180: Logo asset references
  
- **`packages/web-core/src/shared/dialogs/command-bar/CreatePRDialog.tsx`** (1 reference)
  - Line 51: `const PR_TITLE_SUFFIX = ' (vibe-kanban)'`
  
- **`packages/web-core/src/pages/workspaces/PreviewBrowserContainer.tsx`** (1 reference)
  - Line 675: `source: 'vibe-kanban'`
  
- **`packages/web-core/src/shared/actions/index.ts`** (1 reference)
  - Line 859: Comment referencing vibe-kanban identifier
  
- **`packages/web-core/src/shared/lib/relayPake.ts`** (2 references)
  - Lines 5-6: SPAKE2 client/server IDs: `'vibe-kanban-browser'` and `'vibe-kanban-server'`
  
- **`packages/web-core/src/shared/lib/diffDataAdapter.ts`** (3 references)
  - Lines 24, 73, 78: Comments mentioning vibe-kanban

### 2.4 Internationalization Files (i18n)
- **`packages/web-core/src/i18n/locales/en/settings.json`** (2 references)
  - Lines 160, 163: Workspace directory references `.vibe-kanban-workspaces`
  
- **`packages/web-core/src/i18n/locales/zh-Hans/settings.json`** (2 references)
  
- **`packages/web-core/src/i18n/locales/zh-Hant/settings.json`** (2 references)
  
- **`packages/web-core/src/i18n/locales/es/settings.json`** (2 references)
  
- **`packages/web-core/src/i18n/locales/ja/settings.json`** (2 references)
  
- **`packages/web-core/src/i18n/locales/fr/settings.json`** (2 references)
  
- **`packages/web-core/src/i18n/locales/ko/settings.json`** (2 references)

### 2.5 Mock Data & Test Fixtures
- **`packages/web-core/src/mock/normalized_entries.json`** (6 references)
  - Paths in test data referencing `/var/folders/.../T/vibe-kanban-dev/...`
  
- **`packages/web-core/src/test/fixtures/normalized_entries.json`** (6 references)
  - Same as above

### 2.6 Rust Backend
- **`crates/tauri-app/Cargo.toml`** (2 references)
  - Line 2: `name = "vibe-kanban-tauri"`
  - Line 7: Binary name
  
- **`Cargo.lock`** (1 reference)
  - Line 9278: Package name in lock file

### 2.7 Documentation
- **`README.md`** (8 references)
  - Lines 4-6, 13, 22, 42, 51: Logo and package name references
  
- **`docs/index.mdx`** (1 reference)
  - Line 14: `npx vibe-kanban` installation instruction
  
- **`docs/troubleshooting.mdx`** (4 references)
  - Lines 27, 45, 51, 57, 60: Cache paths and log commands
  
- **`docs/settings/general.mdx`** (1 reference)
  - Line 149: Workspace directory configuration
  
- **`docs/settings/mcp-servers.mdx`** (1 reference)
  - Line 7: Reference in documentation
  
- **`docs/core-features/testing-your-application.mdx`** (5 references)
  - Package name `vibe-kanban-web-companion`
  
- **`docs/core-features/creating-tasks.mdx`** (1 reference)
  
- **`docs/integrations/vibe-kanban-mcp-server.mdx`** (multiple references)
  - File name and references to MCP server
  
- **`docs/integrations/mcp-server-configuration.mdx`** (multiple references)
  
- **`docs/integrations/vscode-extension.mdx`** (5+ references)
  - Marketplace links for `bloop.vibe-kanban` extension
  
- **`docs/cloud/index.mdx`** (2 references)
  - Installation instructions
  
- **`docs/cloud/troubleshooting.mdx`** (1 reference)
  
- **`docs/cloud/projects.mdx`** (1 reference)
  - Project abbreviation example "VI"
  
- **`docs/cloud/getting-started.mdx`** (1 reference)
  
- **`docs/workspaces/` (multiple files)** (various references)
  - `.vibe-kanban-workspaces` directory paths
  - Lines in: `creating-workspaces.mdx`, `managing-workspaces.mdx`, `repositories.mdx`
  
- **`docs/configuration-customisation/agent-configurations.mdx`** (1 reference)
  - Card title reference to "Vibe Kanban MCP Server"
  
- **`docs/agents/` (multiple files)** (various references)
  - `npx vibe-kanban` in: `amp.mdx`, `cursor-cli.mdx`, `openai-codex.mdx`, `claude-code.mdx`, `droid.mdx`, `gemini-cli.mdx`, `qwen-code.mdx`, `github-copilot.mdx`, `opencode.mdx`

### 2.8 GitHub Workflows (Build & CI)
- **`.github/workflows/test.yml`** (2 references)
  - Line 251: `--exclude vibe-kanban-tauri`
  - Line 304: Check for vibe-kanban-tauri crate
  
- **`.github/workflows/pre-release.yml`** (12+ references)
  - Binary names: `vibe-kanban-mcp`, `vibe-kanban`, `vibe-kanban-review`
  - Multiple cargo build and artifact copy commands

### 2.9 Build Scripts
- **`local-build.sh`** (11 references)
  - Binary names and zip file names throughout
  
- **`scripts/generate-tauri-update-json.js`** (4 references)
  - Comments about vibe-kanban distribution
  
- **`scripts/generate-desktop-manifest.js`** (4 references)
  - Comments about desktop files

### 2.10 Other Files
- **`mobile-testing.md`** (1 reference)
  - Example application name
  
- **`crates/remote/README.md`** (unknown - needs verification)
  
- **`crates/executors/src/executors/codex/init_prompt.md`** (unknown - needs verification)

---

## 3. Summary Statistics

### Total File Count: **60+** files need updates
### Breakdown by Type:
- **Documentation (Markdown/MDX)**: ~30 files
- **TypeScript/React Code**: ~8 files
- **Rust Code**: ~3 files
- **Configuration (JSON/TOML)**: ~6 files
- **GitHub Workflows**: ~6 files
- **NPX CLI Package**: ~4 files
- **Build Scripts**: ~3 files
- **Internationalization**: ~7 files

### Reference Types:
1. **GitHub URLs** (11 files): Requires org/repo name change
2. **Package names** (8 files): `vibe-kanban` → `kira-code`
3. **Binary names** (5+ files): Build artifacts and executables
4. **Directory paths** (.vibe-kanban-workspaces): Configuration paths
5. **Asset references** (Logo SVG files)
6. **API endpoints** (GitHub API calls)
7. **Configuration identifiers** (Sentry project, SPAKE2 IDs)
8. **VSCode extension IDs** (bloop.vibe-kanban)
9. **CLI commands** (`npx vibe-kanban`)
10. **Comments and documentation strings**

---

## 4. Priority Order for Updates

### Phase 1 (Critical - Public-facing)
1. README.md
2. npx-cli/package.json
3. package.json
4. Main documentation files (docs/index.mdx, docs/getting-started guides)

### Phase 2 (High - API & Configuration)
5. crates/server/src/routes/releases.rs
6. packages/web-core/src/shared/hooks/useGitHubStars.ts
7. packages/web-core/src/shared/dialogs/global/ReleaseNotesDialog.tsx
8. crates/tauri-app/Cargo.toml
9. npx-cli CLI files

### Phase 3 (Medium - Frontend & Branding)
10. Logo asset references
11. LandingPage and onboarding components
12. All documentation markdown files
13. i18n configuration files

### Phase 4 (Low - Internal & CI/CD)
14. GitHub workflow files
15. Build scripts
16. Mock data and test fixtures (may not need changes)
17. Comments in code

---

## 5. Files NOT Changed (Static/Generated)
- `Cargo.lock` - Auto-generated, will update with cargo commands
- `npx-cli/package-lock.json` - Auto-generated, will update with npm commands
- Mock JSON fixtures - Only if paths are actual app behavior
- `.github/workflows/...` internal deployment repos - May need separate coordination

