# Rebrand Summary: KairosUtamaIndonesia/kira-code → Kira Code

## 📊 Executive Summary

This document summarizes the complete rebrand analysis for the transition from **KairosUtamaIndonesia/kira-code** to **Kira Code**.

**Total Files Affected: ~82 files across the repository**

### Key Statistics
- 📖 Documentation files: 36+ 
- 💻 Source code files: 20+ (TypeScript, Rust, JavaScript)
- ⚙️ Configuration files: 8 (package.json, Cargo.toml, JSON)
- 🔄 CI/CD workflows: 6 GitHub Action workflows
- 🌐 i18n translations: 7 language files
- 📝 Build scripts: 3 shell/Node scripts

---

## 🎯 Reference Types to Update

### 1. **GitHub URLs & Organization References**
- GitHub repository URLs: `https://github.com/KairosUtamaIndonesia/kira-code`
- GitHub API endpoints for releases and stars
- GitHub Discussions links
- Workflow repository references to remote deployment repos
- Badge/status URLs

**Files affected: 11 (most critical)**

### 2. **Package & Product Names**
- NPM package name: `vibe-kanban` → `kira-code`
- CLI command: `npx vibe-kanban` → `npx kira-code`
- Rust crate names: `vibe-kanban-tauri`, `vibe-kanban-mcp`, etc.
- Binary names in build scripts
- Sentry project identifiers

**Files affected: 20+**

### 3. **Directory & Path References**
- Workspace directory: `.vibe-kanban-workspaces` → `.kira-code-workspaces`
- Cache directory: `.vibe-kanban/bin` → `.kira-code/bin`
- Temporary paths: `/var/folders/.../T/vibe-kanban` 
- User application data directories (macOS, Linux, Windows)

**Files affected: 8+**

### 4. **Asset & Logo References**
- Logo file names: `vibe-kanban-logo.svg` → `kira-code-logo.svg`
- Logo alt text and image sources
- Screenshot references in documentation

**Files affected: 5+**

### 5. **API & Authentication Identifiers**
- SPAKE2 client/server IDs: `vibe-kanban-browser` → `kira-code-browser`
- GitHub API authentication endpoints
- Relay server identifiers

**Files affected: 2-3**

### 6. **Marketplace & Extension IDs**
- VSCode extension ID: `bloop.vibe-kanban` → `bloop.kira-code` (or similar)
- Open VSX Registry references
- VSCode Marketplace links

**Files affected: 1-2**

### 7. **Documentation & Text References**
- Product names in headings, descriptions, and examples
- Installation instructions mentioning the package name
- Workspace path documentation
- Feature descriptions

**Files affected: 30+**

---

## 📋 Three Reference Documents Created

To help you manage the rebrand, I've created three detailed reference files:

### 1. **`REBRAND_REFERENCES.md`** (Most Detailed)
Comprehensive list organized by reference type showing:
- All 82 files that need updates
- Exact line numbers for each reference
- Description of what needs to change
- Categorized by reference type (URLs, package names, paths, etc.)
- Summary statistics

**Use this for:** Understanding the full scope and detailed planning

### 2. **`REBRAND_CHECKLIST.md`** (Most Actionable)
Phase-by-phase checklist organized by priority:
- **Phase 1:** Critical public-facing changes (README, main docs)
- **Phase 2:** High-priority API & configuration
- **Phase 3:** Frontend branding & onboarding
- **Phase 4:** Documentation updates
- **Phase 5:** CLI & build infrastructure
- **Phase 6:** Test data & generated files
- **Phase 7:** Verification & testing
- **Phase 8:** Final steps & release

**Use this for:** Tracking progress as you execute the rebrand

### 3. **`REBRAND_FILES_BY_TYPE.md`** (Best for Reference)
Files organized by type for quick lookup:
- Configuration files (4)
- Documentation files (36)
- TypeScript/React code (12)
- i18n files (7)
- Rust code (2)
- NPX CLI code (4)
- JSON configs (1)
- Build scripts (3)
- Git config (1)
- Workflows (6)
- Test data (2)

**Use this for:** Finding specific file types quickly

---

## 🚀 Recommended Execution Order

### Stage 1: Preparation (1-2 hours)
1. Create a new git branch for the rebrand
2. Tag current state as "pre-rebrand" checkpoint
3. Review all three reference documents
4. Create asset files (rename logos, create new branding materials)

### Stage 2: Critical Updates (2-3 hours)
1. Update root-level files:
   - `README.md`
   - `package.json`
   - `npx-cli/package.json`

2. Update main documentation:
   - `docs/index.mdx`
   - `docs/getting-started.mdx`
   - `docs/cloud/getting-started.mdx`

3. Update core code:
   - Frontend GitHub links (LandingPage, AppBar, ReleaseNotes)
   - API endpoints (releases, stars)
   - Logo asset references

### Stage 3: Frontend & Branding (2-3 hours)
1. Update all logo references
2. Update i18n translation files (7 languages)
3. Update frontend component references
4. Update onboarding pages

### Stage 4: Documentation (2-4 hours)
1. Update all markdown files in `/docs`
2. Update integration documentation
3. Update agent configuration guides
4. Update self-hosting guides

### Stage 5: Infrastructure (1-2 hours)
1. Update NPX CLI code and build scripts
2. Update GitHub Actions workflows
3. Update Cargo.toml files
4. Update `.gitignore`

### Stage 6: Testing & Validation (2-3 hours)
1. Run format: `pnpm run format`
2. Run linting: `pnpm run lint`
3. Run checks: `pnpm run check`
4. Test local builds
5. Test CLI: `npx kira-code --help`
6. Verify all documentation links

### Stage 7: Release (1-2 hours)
1. Update version number
2. Create release notes
3. Publish to npm
4. Tag release in git
5. Announce rebrand

**Total estimated time: 11-19 hours (depending on coordination needs)**

---

## ⚠️ Important Considerations

### User Data Migration
- Existing installations use `.vibe-kanban-workspaces` directory
- New installations will use `.kira-code-workspaces`
- Consider migration script or user guidance for moving data
- Document the path change in release notes

### External Dependencies
These may require coordination with other teams:
1. **Private repositories:**
   - `KairosUtamaIndonesia/kira-code-private` (in Cargo.toml)
   - May need to rename or update SSH access

2. **Deployment repositories:**
   - `KairosUtamaIndonesia/kira-code-remote-deployment` (6 workflow references)
   - Coordinate with infrastructure/ops team

3. **VSCode Extension:**
   - Check if it needs separate rename
   - Update extension ID if applicable
   - Coordinate with VSCode marketplace team

### Breaking Changes
- New CLI command name (`npx kira-code` instead of `npx vibe-kanban`)
- New workspace directory path
- New GitHub repository location
- Updated package name on npm

**Recommendation:** Include migration guide in release notes

---

## 🔍 Verification Checklist

Before considering the rebrand complete:

- [ ] All GitHub URLs updated to new repository
- [ ] All `npx vibe-kanban` commands updated to `npx kira-code`
- [ ] Logo assets renamed and all references updated
- [ ] i18n files updated for workspace directory paths
- [ ] API endpoints point to correct repository
- [ ] VSCode extension ID updated (if applicable)
- [ ] Documentation links tested and working
- [ ] Binary names reflect new branding
- [ ] Build scripts use new names
- [ ] CI/CD workflows execute successfully
- [ ] NPM package publishes with new name
- [ ] CLI works: `npx kira-code --help`
- [ ] No console errors on app startup
- [ ] GitHub repository settings updated
- [ ] Release notes include migration guidance

---

## 📝 Additional Notes

### Search & Replace Strategy
For bulk updates, you can use find-and-replace with these patterns:

```bash
# Find all occurrences first
grep -r "vibe-kanban" --include="*.ts" --include="*.tsx" --include="*.md" --include="*.mdx" --include="*.json"

# Replace using sed (with backup)
sed -i.bak 's/vibe-kanban/kira-code/g' filename

# Or using find with exec
find . -type f -name "*.md" -exec sed -i 's/vibe-kanban/kira-code/g' {} \;
```

### Cargo.lock and package-lock.json
- These are auto-generated files
- Don't manually edit them
- They'll update with:
  - `cargo build` for Cargo.lock
  - `npm install` or `pnpm install` for package-lock.json

### Code Comments
- Update comments and docstrings that reference the old name
- These are less critical but good for code quality
- Search for TODO comments mentioning vibe-kanban

---

## 🎯 Next Steps

1. **Review the three reference documents** created in this repository:
   - `REBRAND_REFERENCES.md` - Full detailed list
   - `REBRAND_CHECKLIST.md` - Actionable checklist
   - `REBRAND_FILES_BY_TYPE.md` - Files organized by type

2. **Create a git branch** for the rebrand work

3. **Coordinate with stakeholders:**
   - Ops team (for remote deployment repo rename)
   - Marketing team (for branding updates)
   - QA team (for testing plan)

4. **Start with Phase 1** of the checklist (critical changes)

5. **Run tests** after each phase

6. **Document any custom migration steps** needed for users

---

## 📊 Files Summary by Priority

### 🔴 Critical (Update First)
- `README.md` - Public-facing, affects downloads/visibility
- `npx-cli/package.json` - Affects npm registry
- `packages/web-core/src/features/onboarding/ui/LandingPage.tsx` - User-facing
- `packages/web-core/src/shared/hooks/useGitHubStars.ts` - API dependency
- `crates/server/src/routes/releases.rs` - Backend releases
- `docs/docs.json` - Documentation config
- `docs/getting-started.mdx` - First doc users see

### 🟠 High (Update Second)
- All remaining `docs/*.mdx` files
- Frontend components with GitHub links
- TypeScript/React code with package references
- Rust backend files
- NPX CLI code

### 🟡 Medium (Update Third)
- i18n translation files
- Build scripts and workflows
- Configuration files
- Logo and asset references

### 🟢 Low (Update Last)
- Comments in code
- Test fixtures and mock data
- Auto-generated files (will update on next build)

---

## 📞 Support & Resources

For questions about specific files or patterns:
- Refer to `REBRAND_REFERENCES.md` for detailed line numbers
- Refer to `REBRAND_CHECKLIST.md` for phase-by-phase guidance
- Refer to `REBRAND_FILES_BY_TYPE.md` for file organization
- Use `grep` commands provided to find remaining references
- Check git history for context on specific files

---

**Documents Created:**
- ✅ `REBRAND_REFERENCES.md` (11,649 bytes)
- ✅ `REBRAND_CHECKLIST.md` (10,420 bytes)
- ✅ `REBRAND_FILES_BY_TYPE.md` (11,429 bytes)
- ✅ `REBRAND_SUMMARY.md` (this file)

**Total: ~82 files need updates across the repository**

