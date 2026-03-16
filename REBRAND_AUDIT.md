# Vibe Kanban → Kira Code Rebrand Audit

**Generated:** 2026-03-16  
**Total Occurrences:** 450+ across the codebase

---

## Summary by Category

### 1. NPM Package Names (4 locations)
- **Root**: `package.json` - Main monorepo package name: `"name": "vibe-kanban"`
- **npx-cli/package.json** - NPX CLI package: `"name": "vibe-kanban"`
- **npx-cli/package-lock.json** - Locked version of NPX package
- **GitHub Registry**: Referenced in multiple npm-related contexts

### 2. Rust Crate Names (3 locations)
- **crates/mcp/Cargo.toml** - `name = "vibe-kanban-mcp"` (with binary path `src/bin/vibe_kanban_mcp.rs`)
- **crates/tauri-app/Cargo.toml** - `name = "vibe-kanban-tauri"` (with binary name `vibe-kanban-tauri`)
- **Cargo.lock** - References `vibe-kanban-tauri` package lock entry

### 3. Binary Names & Build Artifacts (Multiple in scripts)
- **local-build.sh** (23 occurrences):
  - Build targets: `--bin vibe-kanban-mcp`
  - Output binaries: `vibe-kanban`, `vibe-kanban-mcp`, `vibe-kanban-review`
  - Distribution files: `vibe-kanban.zip`, `vibe-kanban-mcp.zip`, `vibe-kanban-review.zip`
  - Distribution directory: `npx-cli/dist/$PLATFORM/vibe-kanban*.zip`

### 4. GitHub Workflows (60+ occurrences)
- **.github/workflows/pre-release.yml** (45+ occurrences):
  - Binary naming: `vibe-kanban`, `vibe-kanban-mcp`, `vibe-kanban-review`
  - Build matrix configurations
  - Asset packaging and naming
  - NPM version checking: `npm view vibe-kanban version`
  - Tauri binary settings
  
- **.github/workflows/test.yml** (3 occurrences):
  - Exclusion: `--exclude vibe-kanban-tauri`
  - Test configurations for tauri app

- **.github/workflows/relay-deploy-prod.yml** (2 occurrences):
  - Repository dispatch: `KairosUtamaIndonesia/kira-code-remote-deployment`
  - Event type: `vibe-kanban-relay-deploy-prod`

- **.github/workflows/relay-deploy-dev.yml** (2 occurrences):
  - Repository dispatch: `KairosUtamaIndonesia/kira-code-remote-deployment`
  - Event type: `vibe-kanban-relay-deploy-dev`

- **.github/workflows/remote-deploy-dev.yml** (2 occurrences):
  - Repository dispatch: `KairosUtamaIndonesia/kira-code-remote-deployment`
  - Event type: `vibe-kanban-remote-deploy-dev`

- **.github/workflows/remote-deploy-prod.yml** (2 occurrences):
  - Repository dispatch: `KairosUtamaIndonesia/kira-code-remote-deployment`
  - Event type: `vibe-kanban-remote-deploy-prod`

### 5. Directory & Configuration Names (Multiple)
- **.gitignore** (3 occurrences):
  - Line 75: `npx-cli/vibe-kanban-*` - Glob pattern
  - Line 76: `vibe-kanban-*.tgz` - Package archive pattern
  - Line 85: `vibe-kanban-cloud/` - Directory exclusion

- **Config file locations** (Rust):
  - `crates/review/src/config.rs`: Config path `~/.config/vibe-kanban/review.toml`
  - `crates/services/src/services/config/editor/mod.rs`: Config directory reference
  - `crates/services/src/services/filesystem.rs`: `.vibe-kanban-workspaces` subdirectory

- **Cache directory** (TypeScript):
  - `npx-cli/src/download.ts`: Cache dir `~/.vibe-kanban/bin`

### 6. Workspace Directory Pattern
- **Settings & code**: `.vibe-kanban-workspaces` - Used for storing workspace data
  - Rust: `crates/services/src/services/filesystem.rs`
  - TypeScript i18n: All locale settings files mention this path
  - Documentation: `docs/settings/general.mdx`

### 7. Branding Text in Code (10+ files)
#### React/TypeScript Components:
- **packages/web-core/src/shared/hooks/usePageTitle.ts**: `const BASE_TITLE = 'Vibe Kanban'`
- **packages/local-web/index.html**: `<title>Vibe Kanban</title>`
- **packages/remote-web/index.html**: `<title>Vibe Kanban Remote</title>`
- **npx-cli/README.md**: Multiple instances of "Vibe Kanban" branding
- **npx-cli/src/desktop.ts**: User-facing strings like "Installing Vibe Kanban...", "Launch Vibe Kanban"
- **npx-cli/src/cli.ts**: CLI descriptions and launch messages

#### Rust Code:
- **crates/tauri-app/src/main.rs**: Window title `.title("Vibe Kanban")`
- **crates/git/src/lib.rs**: Git committer identity `"Vibe Kanban"` with email `"noreply@kira-code.kairos-it.com"`
- **crates/server/src/routes/oauth.rs**: HTML in OAuth pages: `alt="Vibe Kanban"`
- **crates/review/src/main.rs**: App description mentions "Vibe-Kanban"

### 8. Logo & Asset Files (7 locations)
- **packages/public/vibe-kanban-logo.svg** - Light theme logo
- **packages/public/vibe-kanban-logo-dark.svg** - Dark theme logo
- **packages/public/vibe-kanban-screenshot-overview.png** - Product screenshot
- **packages/public/vibe-kanban-screenshot-workspace.png** - Workspace screenshot
- **docs/images/vibe-kanban-screenshot-overview.png** - Documentation screenshot
- **crates/tauri-app/splash/index.html**: References logos

#### Referenced in code (15+ files):
- **packages/web-core/src/features/onboarding/ui/LandingPage.tsx**: Logo src paths
- **packages/web-core/src/features/onboarding/ui/OnboardingSignInPage.tsx**: Logo src paths
- **packages/web-core/src/pages/migrate/MigratePage.tsx**: Logo src paths
- **packages/remote-web/src/shared/components/BrandLogo.tsx**: Logo component
- **README.md**: Multiple logo references in SVG picture element

### 9. URLs & Domains (20+ occurrences)

#### API & Service URLs:
- `https://api.kira-code.kairos-it.com` - API endpoint (local-build.sh)
- `https://cloud.kira-code.kairos-it.com` - Cloud instance
- `https://relay.kira-code.kairos-it.com` - Relay server
- `https://www.kira-code.kairos-it.com` - Main website (docs, terms, privacy)
- `https://www.kira-code.kairos-it.com/docs` - Documentation
- `https://www.kira-code.kairos-it.com/docs/getting-started` - Getting started guide

#### Repository URLs:
- `https://github.com/KairosUtamaIndonesia/kira-code` - Main GitHub repo (4 files)
- `https://github.com/KairosUtamaIndonesia/kira-code/releases` - Release endpoint
- `https://github.com/KairosUtamaIndonesia/kira-code/discussions` - Discussions
- `KairosUtamaIndonesia/kira-code-remote-deployment` - Deployment repository (in CI/CD)
- `https://api.github.com/repos/KairosUtamaIndonesia/kira-code` - GitHub API calls

#### Documentation URLs:
- Multiple `.kira-code.kairos-it.com` domain references in doc files
- Hardcoded in TypeScript/React components

### 10. Internationalization (i18n) - Multiple Locale Files
**27 files** in `packages/web-core/src/i18n/locales/` with brand references:

#### Locale directories:
- **en/** (English): `common.json`, `settings.json`, `tasks.json`
- **es/** (Spanish): `common.json`, `settings.json`, `tasks.json`
- **fr/** (French): `common.json`, `settings.json`, `tasks.json`
- **ja/** (Japanese): `common.json`, `settings.json`, `tasks.json`
- **ko/** (Korean): `common.json`, `settings.json`, `tasks.json`
- **zh-Hans/** (Chinese Simplified): `common.json`, `settings.json`, `tasks.json`
- **zh-Hant/** (Chinese Traditional): `common.json`, `settings.json`, `tasks.json`

#### Content patterns in i18n files:
- "Sign in to Vibe Kanban" / "Vibe Kanban にサインイン" (title)
- "Welcome to Vibe Kanban" / "欢迎使用 Vibe Kanban" (onboarding)
- ".vibe-kanban-workspaces" (directory path)
- "Vibe-Kanban" (hyphenated, in settings)
- "Help improve Vibe-Kanban" (in telemetry settings)

### 11. Documentation Files (35+ files)
#### Markdown/MDX files:
- **README.md** (11 occurrences): Badges, links, branding, screenshots
- **npx-cli/README.md** (18 occurrences): Full NPM package documentation
- **docs/integrations/vibe-kanban-mcp-server.mdx** - Integration guide
- **docs/responsible-disclosure.mdx** - Security policy
- **docs/remote-access.mdx** - Feature documentation
- **docs/settings/** (6 files): General, MCP servers, organization, projects, agent configs
- **docs/core-features/** (4 files): Testing, creating tasks, monitoring
- **docs/agents/** (11 files): Agent documentation
- **docs/cloud/** (4 files): Cloud features
- **docs/workspaces/** (3 files): Workspace management
- **mobile-testing.md** - Mobile testing guide

### 12. Environment Variables & Secrets
- **local-build.sh**: 
  - `VK_SHARED_API_BASE="https://api.kira-code.kairos-it.com"`
  - `VITE_VK_SHARED_API_BASE="https://api.kira-code.kairos-it.com"`
  - Environment variable: `VIBE_KANBAN_DEBUG`

### 13. Configuration & Metadata Files
- **packages/public/site.webmanifest**: `"name": "Vibe Kanban"`
- **crates/tauri-app/tauri.conf.json**: Referenced in various configs
- **crates/tauri-app/capabilities/default.json**: `"description": "Default capabilities for Vibe Kanban desktop app"`
- **crates/tauri-app/gen/schemas/capabilities.json**: Generated schema reference
- **crates/executors/default_mcp.json**: MCP configuration
- **docs/docs.json**: Documentation metadata

### 14. Sentry & Analytics Integration
- **packages/local-web/vite.config.ts**: 
  - `org: 'bloop-ai'`
  - `project: 'vibe-kanban'`

### 15. NPX CLI Specifics
- **npx-cli/src/cli.ts** (8 occurrences):
  - `const cli = cac("vibe-kanban")`
  - Command descriptions
  - Version checking
  - Extraction commands
  
- **npx-cli/src/desktop.ts** (8 occurrences):
  - Windows app name: `'Vibe Kanban.exe'`
  - Installation messages
  - Launch messages
  - Start menu references

- **npx-cli/src/download.ts** (2 occurrences):
  - Cache directory path
  - Environment variable `VIBE_KANBAN_LOCAL`

### 16. Communication Protocol Constants
- **crates/trusted-key-auth/src/spake2.rs** (2 occurrences):
  - `const SPAKE2_CLIENT_ID: &[u8] = b"vibe-kanban-browser"`
  - `const SPAKE2_SERVER_ID: &[u8] = b"vibe-kanban-server"`

- **packages/web-core/src/shared/lib/relayPake.ts** (2 occurrences):
  - Same constants in TypeScript/JavaScript equivalent

### 17. Miscellaneous Code References
- **packages/web-core/src/shared/dialogs/command-bar/CreatePRDialog.tsx**: 
  - PR title suffix: `' (vibe-kanban)'`

- **packages/web-core/src/shared/dialogs/global/ReleaseNotesDialog.tsx**: 
  - GitHub releases URL construction

- **crates/server/src/routes/releases.rs**: 
  - GitHub API endpoint: `https://api.github.com/repos/KairosUtamaIndonesia/kira-code/releases`
  - User agent: `"vibe-kanban-server"`

- **crates/server/src/routes/workspaces/git.rs**: 
  - Function: `resolve_vibe_kanban_identifier()`

- **crates/mcp/src/bin/vibe_kanban_mcp.rs**: 
  - Binary source file

- **crates/mcp/src/task_server/handler.rs**: 
  - Server description: "A Vibe Kanban MCP server..."
  - Server name: `"vibe-kanban-mcp"`

- **crates/review/src/main.rs**: 
  - Default API: `https://api.kira-code.kairos-it.com`
  - App description

- **crates/server/src/preview_proxy/eruda_init.js**: 
  - Command source: `'vibe-kanban'`

- **crates/services/src/services/qa_repos.rs**: 
  - Configuration reference

- **crates/utils/src/assets.rs**, **path.rs**, **port_file.rs**: 
  - Path handling for vibe-kanban directories

- **crates/local-deployment/src/pty.rs**: 
  - Log file naming

- **crates/executors/src/executors/acp/session.rs**: 
  - Session management

- **crates/remote/src/** (3 files): 
  - GitHub app service references
  - Auth provider configurations
  - App context

- **crates/git/tests/git_workflow.rs** (2 occurrences): 
  - Test assertions for git committer name and email
  - `"Vibe Kanban"` and `"noreply@kira-code.kairos-it.com"`

### 18. Test Data & Mock Files
- **packages/web-core/src/test/fixtures/normalized_entries.json** (3 occurrences):
  - Mock file paths containing `/T/vibe-kanban-dev/worktrees/`

- **packages/web-core/src/mock/normalized_entries.json** (3 occurrences):
  - Same mock data

### 19. Asset Names in Scripts
- **assets/scripts/toast-notification.ps1**: 
  - PowerShell script: `[string]$AppName = "Vibe Kanban"`

- **scripts/generate-tauri-update-json.js** (8 comments):
  - Example build artifacts with vibe-kanban naming

---

## File Count by Type

| Category | Count |
|----------|-------|
| TypeScript/JavaScript files | 25 |
| Rust files | 27 |
| Markdown/MDX documentation | 35+ |
| JSON configuration files | 15+ |
| i18n locale files | 27 |
| YAML workflow files | 8 |
| Shell scripts | 2 |
| SVG/PNG assets | 7 |
| HTML files | 2 |
| Other config files | 5+ |

**Total: 150+ distinct files affected**

---

## Key Rebrand Points to Address

### Critical Changes Needed:
1. ✅ **NPM Package Names** - Update root `package.json` and `npx-cli/package.json`
2. ✅ **Rust Crate Names** - Update `Cargo.toml` files and binary paths
3. ✅ **Logo Files** - Rename 4 SVG/PNG assets
4. ✅ **GitHub Repository** - Rename repo and update all references
5. ✅ **GitHub Workflows** - Update binary names and deployment references
6. ✅ **Configuration Directories** - Change `.vibe-kanban-workspaces` pattern
7. ✅ **API Endpoints** - Update domain/URL references
8. ✅ **Git Committer Identity** - Update git config and email
9. ✅ **All i18n Strings** - Update across all 7 locales
10. ✅ **Documentation** - Rebrand all 35+ doc files
11. ✅ **Environment Variables** - Rename `VIBE_KANBAN_*` variables
12. ✅ **Sentry Project** - Update analytics project name
13. ✅ **Desktop App** - Update window titles and installer names
14. ✅ **Brand Strings** - Update "Vibe Kanban" text throughout UI
15. ✅ **URL/Domain References** - Update all hardcoded URLs

### Secondary Changes:
- Update git submodule for `vibe-kanban-remote-deployment`
- Update GitHub Actions dispatch event types
- Update cache directory naming
- Update PR title suffix
- Update error messages and help text
- Update CLI descriptions
- Update wireless protocol constants (SPAKE2 identifiers)

---

## Implementation Strategy

### Phase 1: Core Infrastructure
1. Rename GitHub repository
2. Update Cargo.toml crate names
3. Update package.json files
4. Update NPM package registry

### Phase 2: Binaries & Build
1. Rename binary names in build scripts
2. Update GitHub Actions workflows
3. Rename shell script references
4. Update Sentry configuration

### Phase 3: Configuration & Paths
1. Update directory patterns (`.vibe-kanban-workspaces` → `.kira-code-workspaces`)
2. Update config file paths
3. Update cache directory paths
4. Update environment variable names

### Phase 4: Branding & Documentation
1. Update i18n files (all 7 locales)
2. Update documentation (35+ files)
3. Update logo asset references in code
4. Update URL references and domains

### Phase 5: API & Services
1. Update API endpoint domains
2. Update git committer identity
3. Update communication protocol constants
4. Update database/service references

### Phase 6: Testing & Validation
1. Run full test suite
2. Verify all URLs are updated
3. Test CLI commands
4. Test desktop app installation
5. Verify i18n rendering in all locales

