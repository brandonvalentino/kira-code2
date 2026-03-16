# Files to Update for Rebrand: Organized by Type

Quick reference guide showing all files that need updates, organized by file type.

---

## 📋 Configuration Files (package.json, Cargo.toml)

### NPM/Node Configuration
1. **`package.json`** (Root)
   - Line 2: Package name
   - Line 6: CLI bin mapping
   
2. **`npx-cli/package.json`**
   - Line 2: Package name
   - Line 7: Bin mapping
   - Line 17: Repository URL (GitHub)
   - Line 23: Description text

### Rust Configuration
3. **`crates/tauri-app/Cargo.toml`**
   - Line 2: Package name
   - Line 7: Binary name

4. **`crates/remote/Cargo.toml`**
   - Line 17: Git dependency (private repo)

---

## 📖 Documentation (Markdown/MDX Files)

### Root Documentation
5. **`README.md`** ⭐ CRITICAL
   - Lines 4-6: Logo source images
   - Line 13: NPM badge
   - Line 14: Build status badge
   - Line 15: DeepWiki badge
   - Line 22: Screenshot reference
   - Line 42: Installation command
   - Line 51: Installation command
   - Line 64: GitHub Discussions link
   - Line 68: GitHub Discussions link

### Getting Started & Troubleshooting
6. **`docs/index.mdx`** ⭐ CRITICAL
   - Line 14: Installation command

7. **`docs/getting-started.mdx`**
   - Installation command references

8. **`docs/troubleshooting.mdx`**
   - Line 27: `npx vibe-kanban` command
   - Line 45: macOS path with vibe-kanban
   - Line 51: Linux path
   - Line 57: Windows path
   - Line 60: Windows path example

9. **`docs/responsible-disclosure.mdx`**
   - Check for any references

### Cloud Documentation
10. **`docs/cloud/getting-started.mdx`**
    - Installation command

11. **`docs/cloud/index.mdx`**
    - Multiple `npx vibe-kanban` references

12. **`docs/cloud/troubleshooting.mdx`** ⭐ CRITICAL
    - Line 270: Restart command
    - Line 296: GitHub issues link
    - Line 303: Report issue card href

13. **`docs/cloud/projects.mdx`**
    - Line 35: Project abbreviation example

### Configuration & Settings
14. **`docs/configuration-customisation/global-settings.mdx`**
    - Workspace directory references

15. **`docs/settings/general.mdx`**
    - Line 149: Workspace directory config

### Workspace Management
16. **`docs/workspaces/creating-workspaces.mdx`**
    - Workspace directory references

17. **`docs/workspaces/managing-workspaces.mdx`**
    - Lines 102-106: Path examples
    - Line 113: macOS command
    - Line 118: Linux command
    - Line 123: Windows command

18. **`docs/workspaces/repositories.mdx`**
    - Workspace configuration references

19. **`docs/workspaces/index.mdx`**
    - Check for references

### Integrations
20. **`docs/integrations/vibe-kanban-mcp-server.mdx`** ⭐ RENAME FILE
    - Entire file about Vibe Kanban MCP Server
    - Line 47: `npx vibe-kanban@latest --mcp`
    - Line 53: Help about --mcp argument

21. **`docs/integrations/mcp-server-configuration.mdx`**
    - References to Vibe Kanban

22. **`docs/integrations/vscode-extension.mdx`**
    - VSCode marketplace links with `bloop.vibe-kanban` ID
    - Open VSX Registry links
    - Search instructions with extension ID

### Core Features
23. **`docs/core-features/testing-your-application.mdx`**
    - Lines 49, 63, 72, 90, 107: Package name `vibe-kanban-web-companion`

24. **`docs/core-features/creating-tasks.mdx`**
    - Reference to Vibe Kanban MCP Server

### Self-Hosting & Deployment
25. **`docs/self-hosting/local-development.mdx`** ⭐ CRITICAL
    - Line 20: `git clone https://github.com/KairosUtamaIndonesia/kira-code.git`
    - Line 21: `cd vibe-kanban`

26. **`docs/self-hosting/deploy-docker.mdx`** ⭐ CRITICAL
    - Line 33: `git clone` URL
    - Line 34: `cd vibe-kanban`
    - Line 259: `cd vibe-kanban`

### Agent Integration Docs
27. **`docs/agents/amp.mdx`**
    - `npx vibe-kanban` command

28. **`docs/agents/cursor-cli.mdx`**
    - `npx vibe-kanban` command

29. **`docs/agents/openai-codex.mdx`**
    - `npx vibe-kanban` commands

30. **`docs/agents/claude-code.mdx`**
    - `npx vibe-kanban` command

31. **`docs/agents/droid.mdx`**
    - `npx vibe-kanban` command

32. **`docs/agents/gemini-cli.mdx`**
    - `npx vibe-kanban` command

33. **`docs/agents/qwen-code.mdx`**
    - `npx vibe-kanban` command

34. **`docs/agents/github-copilot.mdx`**
    - `npx vibe-kanban` command

35. **`docs/agents/opencode.mdx`**
    - `npx vibe-kanban` command

36. **`docs/agents/ccr.mdx`**
    - Check for references

### Agent Configuration
37. **`docs/configuration-customisation/agent-configurations.mdx`**
    - Card title reference to "Vibe Kanban MCP Server"

### Other Documentation
38. **`docs/README.md`**
    - Check for references

39. **`docs/reviewing-code.mdx`**
    - Check for references

40. **`mobile-testing.md`** ⭐ Root level
    - Line 139: Example app name

---

## 🔧 TypeScript/React Source Code

### Frontend - Web Core
41. **`packages/web-core/src/features/onboarding/ui/LandingPage.tsx`** ⭐ CRITICAL
    - Line 117: GitHub href
    - Lines 179-180: Logo asset references

42. **`packages/web-core/src/features/onboarding/ui/OnboardingSignInPage.tsx`**
    - Lines 99-100: Logo asset references

43. **`packages/web-core/src/pages/migrate/MigratePage.tsx`**
    - Lines 49-50: Logo asset references

44. **`packages/web-core/src/pages/workspaces/PreviewBrowserContainer.tsx`**
    - Line 675: Source identifier

45. **`packages/web-core/src/shared/dialogs/command-bar/CreatePRDialog.tsx`**
    - Line 51: PR title suffix

46. **`packages/web-core/src/shared/dialogs/global/ReleaseNotesDialog.tsx`** ⭐ CRITICAL
    - Line 15: GitHub releases URL

47. **`packages/web-core/src/shared/hooks/useGitHubStars.ts`** ⭐ CRITICAL
    - Line 6: GitHub API endpoint

48. **`packages/web-core/src/shared/actions/index.ts`**
    - Line 859: Comment about vibe-kanban identifier

49. **`packages/web-core/src/shared/lib/relayPake.ts`**
    - Lines 5-6: SPAKE2 client/server IDs

50. **`packages/web-core/src/shared/lib/diffDataAdapter.ts`**
    - Lines 24, 73, 78: Comments referencing vibe-kanban

### Frontend - UI Components
51. **`packages/ui/src/components/AppBar.tsx`** ⭐ CRITICAL
    - Line 392: GitHub link href

### Frontend - Remote Web
52. **`packages/remote-web/src/shared/components/BrandLogo.tsx`**
    - Lines 13, 16: Logo asset references

### Frontend - Build Configuration
53. **`packages/local-web/vite.config.ts`**
    - Line 111: Sentry project configuration

---

## 🌐 Internationalization (i18n) Files

All in `packages/web-core/src/i18n/locales/{language}/settings.json`:

54. **`en/settings.json`**
    - Lines 160, 163: Workspace directory helper text

55. **`zh-Hans/settings.json`**
    - Lines 160, 163: Chinese Simplified

56. **`zh-Hant/settings.json`**
    - Lines 160, 163: Chinese Traditional

57. **`es/settings.json`**
    - Lines 160, 163: Spanish

58. **`ja/settings.json`**
    - Lines 160, 163: Japanese

59. **`fr/settings.json`**
    - Lines 160, 163: French

60. **`ko/settings.json`**
    - Lines 160, 163: Korean

---

## ⚙️ Rust Source Code

### Routes & API
61. **`crates/server/src/routes/releases.rs`** ⭐ CRITICAL
    - Line 14: GitHub API URL constant

### Test Utilities
62. **`crates/remote/README.md`**
    - Check for references

---

## ⚡ NPX CLI Code

63. **`npx-cli/src/cli.ts`**
    - Line 209: Update notification text
    - Line 217: Extract command for vibe-kanban-mcp
    - Line 234: Extract command for vibe-kanban-review
    - Line 255: Startup message
    - Line 276: Extract command for vibe-kanban
    - Line 310: CLI name
    - Line 313: Command description

64. **`npx-cli/src/desktop.ts`**
    - Line 238: Command/label reference

65. **`npx-cli/src/download.ts`**
    - Line 10: Cache directory path `.vibe-kanban`
    - Line 202: Update path reference

66. **`npx-cli/README.md`**
    - Lines 10, 18-21, 179: Installation command examples

---

## 📋 JSON Configuration Files

67. **`docs/docs.json`** ⭐ CRITICAL
    - Line 138: GitHub href in integrations
    - Line 177: GitHub field in config

---

## 🔨 Build & Script Files

### Shell Scripts
68. **`local-build.sh`**
    - Line 58: Binary name vibe-kanban-mcp
    - Line 63-72: Multiple binary name references
    - Line 82-84: Artifact path references

### Node/JavaScript Scripts
69. **`scripts/generate-tauri-update-json.js`**
    - Line 10: Comment with GitHub download URL

70. **`scripts/generate-desktop-manifest.js`**
    - Lines 15-19: Comments with binary names

### Script Index
71. **`scripts/relay-test-client/index.html`**
    - Lines 224-225: SPAKE2 IDs

---

## 🔄 Git Configuration

72. **`.gitignore`**
    - Line 75: `npx-cli/vibe-kanban-*` pattern
    - Line 76: `vibe-kanban-*.tgz` pattern
    - Line 85: `vibe-kanban-cloud/` directory

---

## 🔐 GitHub Actions Workflows

### CI/Testing
73. **`.github/workflows/test.yml`**
    - Line 251: Exclude vibe-kanban-tauri from clippy
    - Line 304: Check vibe-kanban-tauri crate

### Pre-Release & Build
74. **`.github/workflows/pre-release.yml`**
    - Multiple references to:
      - Binary names: vibe-kanban, vibe-kanban-mcp, vibe-kanban-review
      - Artifact copying and naming
      - Cargo build commands

### Deployment Workflows
75. **`.github/workflows/relay-deploy-dev.yml`**
    - Line 22: Remote deployment repo name

76. **`.github/workflows/relay-deploy-prod.yml`**
    - Line 101: Remote deployment repo name

77. **`.github/workflows/remote-deploy-dev.yml`**
    - Line 23: Remote deployment repo name

78. **`.github/workflows/remote-deploy-prod.yml`**
    - Line 109: Remote deployment repo name

---

## 📦 Mock Data & Test Fixtures

79. **`packages/web-core/src/mock/normalized_entries.json`**
    - Multiple references in test data paths (vibe-kanban-dev)

80. **`packages/web-core/src/test/fixtures/normalized_entries.json`**
    - Multiple references in test fixture paths

---

## 🔒 Generated/Lock Files (Auto-Update)

81. **`Cargo.lock`**
    - Will auto-update with `cargo build`

82. **`npx-cli/package-lock.json`**
    - Will auto-update with `npm install`

---

## Quick Search Commands

Find remaining references:
```bash
# All vibe-kanban references
grep -r "vibe-kanban" /home/brandon/projects/kira-code2 \
  --include="*.ts" --include="*.tsx" --include="*.md" --include="*.mdx" \
  --include="*.json" --include="*.toml" --include="*.js" --include="*.sh" \
  --include="*.yml" --include="*.yaml" | grep -v node_modules | grep -v ".next"

# BloopAI organization references  
grep -r "BloopAI" /home/brandon/projects/kira-code2 \
  --include="*.ts" --include="*.tsx" --include="*.md" --include="*.mdx" \
  --include="*.json" --include="*.toml" --include="*.js" --include="*.sh" \
  --include="*.yml" --include="*.yaml" | grep -v node_modules | grep -v ".next"

# Bloop branding references
grep -r "bloop\.vibe-kanban\|bloop-ai" /home/brandon/projects/kira-code2 \
  --include="*.ts" --include="*.tsx" --include="*.md" --include="*.mdx" \
  --include="*.json" --include="*.toml" --include="*.js" --include="*.sh" \
  --include="*.yml" --include="*.yaml" | grep -v node_modules | grep -v ".next"
```

---

## Summary Statistics

| Category | Count |
|----------|-------|
| Configuration Files | 4 |
| Documentation (MD/MDX) | 36 |
| TypeScript/React Code | 12 |
| i18n JSON Files | 7 |
| Rust Code | 2 |
| NPX CLI Code | 4 |
| JSON Config | 1 |
| Build Scripts | 3 |
| Git Config | 1 |
| GitHub Workflows | 6 |
| Mock/Test Data | 2 |
| **TOTAL** | **~82 files** |

**Files that need updates: 60-82 depending on scope (test data, comments, etc.)**

