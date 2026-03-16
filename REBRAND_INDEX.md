# Rebrand Documentation Index

**Start here for a complete guide to rebranding from KairosUtamaIndonesia/kira-code to Kira Code.**

---

## 📚 Four Core Documents

### 1. **REBRAND_SUMMARY.md** ← START HERE
**Purpose:** Executive overview and roadmap
- 📊 Statistics on files affected
- 🎯 Reference types to update
- 🚀 Recommended execution order (7 stages)
- ⏱️ Estimated time (11-19 hours)
- ⚠️ Important considerations
- 🔍 Verification checklist

**Best for:** Understanding the big picture, planning timeline

---

### 2. **REBRAND_CHECKLIST.md** ← USE DURING EXECUTION
**Purpose:** Phase-by-phase actionable checklist
- ✅ 8 phases with individual checkboxes
- 🔴 Phase 1: Critical public-facing changes
- 🟠 Phase 2: High-priority API & configuration
- 🟡 Phases 3-8: Progressive refinement
- 📝 Detailed guidance for each file
- 💡 Notes on search commands and migration

**Best for:** Tracking progress, managing execution

---

### 3. **REBRAND_REFERENCES.md** ← REFERENCE DURING UPDATES
**Purpose:** Complete detailed reference with line numbers
- 🔗 Direct GitHub repository references (11 files)
- 🏷️ Indirect references (vibe-kanban identifiers, paths, etc.)
- 📈 Summary statistics by file type
- 🎯 Priority order for updates
- 📋 Section on files NOT changed

**Best for:** Finding exact locations, understanding context

---

### 4. **REBRAND_FILES_BY_TYPE.md** ← QUICK FILE LOOKUP
**Purpose:** Files organized by type with line numbers
- 📋 Configuration files (4)
- 📖 Documentation files (36)
- 🔧 TypeScript/React code (12)
- 🌐 i18n files (7)
- ⚙️ Rust code (2)
- ⚡ NPX CLI code (4)
- 🔨 Build & scripts (3)
- 🔄 GitHub workflows (6)
- Plus: Mock data, test fixtures, auto-generated files

**Best for:** Finding specific file types quickly

---

## 🗺️ How to Use These Documents

### If you're starting the rebrand:
1. Read **REBRAND_SUMMARY.md** (10 min)
2. Create a git branch
3. Review **REBRAND_CHECKLIST.md** Phase 1 (5 min)
4. Start executing Phase 1 updates

### If you're looking for a specific file:
1. Check **REBRAND_FILES_BY_TYPE.md** 
2. Find line numbers in that file
3. Look up context in **REBRAND_REFERENCES.md** if needed

### If you're in the middle of execution:
1. Use **REBRAND_CHECKLIST.md** as your primary guide
2. Reference **REBRAND_REFERENCES.md** for exact locations
3. Consult **REBRAND_FILES_BY_TYPE.md** for file organization

### If you need to find something specific:
1. Search the documents using Ctrl+F
2. Use the grep commands in **REBRAND_SUMMARY.md**
3. Check **REBRAND_REFERENCES.md** for cross-references

---

## ⚡ Quick Stats

| Category | Count |
|----------|-------|
| **Total Files** | ~82 |
| **Documentation Files** | 36+ |
| **Source Code Files** | 20+ |
| **Configuration Files** | 8 |
| **Workflow Files** | 6 |
| **i18n Files** | 7 |
| **Build Scripts** | 3 |
| **Estimated Time** | 11-19 hours |

---

## 🎯 High-Level Phases

### Phase 1: Critical (2-3 hours)
- [ ] README.md
- [ ] package.json
- [ ] npx-cli/package.json
- [ ] Core documentation
- [ ] Frontend GitHub links

### Phase 2: High-Priority (2-3 hours)
- [ ] API endpoints
- [ ] Rust backend
- [ ] Release URLs
- [ ] Configuration files

### Phase 3: Frontend (2-3 hours)
- [ ] Logo assets
- [ ] Onboarding pages
- [ ] Component references
- [ ] i18n files

### Phase 4: Documentation (2-4 hours)
- [ ] All /docs files
- [ ] Integration guides
- [ ] Deployment docs
- [ ] Agent configs

### Phase 5: Infrastructure (1-2 hours)
- [ ] NPX CLI code
- [ ] Build scripts
- [ ] Workflows
- [ ] .gitignore

### Phase 6: Testing (2-3 hours)
- [ ] Format code
- [ ] Run linting
- [ ] Type checking
- [ ] Build testing

### Phase 7: Release (1-2 hours)
- [ ] Version updates
- [ ] Release notes
- [ ] npm publish
- [ ] Announcement

---

## 📖 Document Contents Overview

### REBRAND_SUMMARY.md
- Executive summary
- Reference types
- Execution roadmap
- Recommended phases
- Verification checklist
- Migration considerations

### REBRAND_CHECKLIST.md
- Phase 1: Critical changes (README, package.json, main docs)
- Phase 2: API & configuration (GitHub integration, Rust backend)
- Phase 3: Frontend branding (logos, components, onboarding)
- Phase 4: Documentation (all .mdx files, i18n)
- Phase 5: Build infrastructure (CLI, scripts, workflows)
- Phase 6: Testing & verification
- Phase 7: Release & publishing
- Phase 8: Post-rebrand steps
- Notes and search commands

### REBRAND_REFERENCES.md
- 11 files with direct GitHub URLs
- 50+ files with vibe-kanban identifiers
- Exact line numbers for each reference
- Description of what needs changing
- 5 priority phases
- Files NOT to change

### REBRAND_FILES_BY_TYPE.md
- Configuration files (package.json, Cargo.toml)
- Documentation (36+ markdown/MDX files)
- TypeScript/React source code
- Internationalization files
- Rust backend code
- NPX CLI code
- JSON configs
- Build scripts
- Workflows
- Test data
- Summary with search commands

---

## 🔍 Key Reference Information

### Main Changes Required:
1. `KairosUtamaIndonesia/kira-code` → New org/repo
2. `vibe-kanban` → `kira-code` (package names)
3. `npx vibe-kanban` → `npx kira-code` (CLI)
4. `.vibe-kanban-workspaces` → `.kira-code-workspaces` (paths)
5. `vibe-kanban-logo.svg` → `kira-code-logo.svg` (assets)
6. `bloop.vibe-kanban` → `bloop.kira-code` (VSCode extension)

### File Types to Update:
- ✅ Markdown (.md, .mdx) - 36+ files
- ✅ TypeScript/React (.ts, .tsx) - 12+ files
- ✅ JSON (.json) - 8+ files
- ✅ Rust (.rs, Cargo.toml) - 3+ files
- ✅ Shell scripts (.sh) - 1 file
- ✅ JavaScript (.js) - 2 files
- ✅ YAML (.yml) - 6 files

### Do NOT Change:
- ❌ Cargo.lock (auto-generated)
- ❌ package-lock.json (auto-generated)
- ❌ Test fixtures (unless needed for app behavior)
- ❌ Comments-only references (unless desired)

---

## 🚀 Quick Start

### 1. Get Oriented (15 minutes)
```bash
# View the summary
cat REBRAND_SUMMARY.md | head -50

# Understand the scope
cat REBRAND_REFERENCES.md | head -100

# Plan your execution
cat REBRAND_CHECKLIST.md
```

### 2. Set Up (30 minutes)
```bash
# Create a feature branch
git checkout -b rebrand/kira-code

# Create a save point
git tag pre-rebrand-kira-code

# Prepare asset files (rename logos, etc.)
```

### 3. Execute (8-16 hours)
- Follow **REBRAND_CHECKLIST.md** phases
- Reference exact locations in **REBRAND_REFERENCES.md**
- Use **REBRAND_FILES_BY_TYPE.md** for quick lookups
- Run tests after each phase

### 4. Verify (2-3 hours)
```bash
# Format all code
pnpm run format

# Lint
pnpm run lint

# Type check
pnpm run check

# Build
pnpm run dev

# Test CLI
npx kira-code --help
```

### 5. Release (1-2 hours)
- Update version and CHANGELOG
- Create git tag
- Publish to npm
- Announce rebrand

---

## 📞 Common Questions

**Q: Where do I start?**
A: Read REBRAND_SUMMARY.md first, then follow REBRAND_CHECKLIST.md Phase 1

**Q: How long will this take?**
A: 11-19 hours depending on team size and coordination needs

**Q: Which files are most critical?**
A: README.md, package.json, npx-cli/package.json, main documentation, GitHub API endpoints

**Q: Do I need to update test data?**
A: Only if it affects user-facing behavior; mock data can usually stay unchanged

**Q: What about the GitHub repository rename?**
A: Update URLs in code and docs, then coordinate the actual GitHub org/repo rename

**Q: Are there any breaking changes?**
A: Yes - new CLI command name and workspace directory path; include migration guide

**Q: Do I need to update lock files?**
A: No, they auto-generate on the next `cargo build` or `npm install`

---

## 🔗 File Cross-References

### Core Application Files
- **Entry point:** `README.md` → `npx-cli/package.json` → `package.json`
- **Frontend:** `packages/web-core/src/` (most frontend changes here)
- **Backend:** `crates/server/`, `crates/tauri-app/`
- **CLI:** `npx-cli/src/`

### Documentation Structure
- **Getting started:** `docs/index.mdx` → `docs/getting-started.mdx`
- **Cloud docs:** `docs/cloud/getting-started.mdx` → other cloud files
- **Integrations:** `docs/integrations/` (6+ files)
- **Deployment:** `docs/self-hosting/`
- **Agents:** `docs/agents/` (9 files)

---

## ✅ Success Criteria

After completing the rebrand, you should be able to:

1. ✅ Run `npx kira-code --help` successfully
2. ✅ All documentation links work
3. ✅ GitHub API calls succeed
4. ✅ No hardcoded "vibe-kanban" references in user-facing text
5. ✅ New workspaces use `.kira-code-workspaces` path
6. ✅ npm package publishes as `kira-code`
7. ✅ Build passes: `pnpm run check` & `pnpm run lint`
8. ✅ GitHub workflows execute successfully
9. ✅ VSCode extension works (if applicable)
10. ✅ Release notes include migration guidance

---

## 📋 Documents in This Package

1. **REBRAND_INDEX.md** (this file) - Navigation guide
2. **REBRAND_SUMMARY.md** - Executive overview and roadmap
3. **REBRAND_CHECKLIST.md** - Actionable 8-phase checklist
4. **REBRAND_REFERENCES.md** - Detailed file reference with line numbers
5. **REBRAND_FILES_BY_TYPE.md** - Files organized by type

**Total Size:** ~45,000 bytes of documentation
**File Count:** ~82 files need updates
**Estimated Time:** 11-19 hours

---

## 🎯 Next Steps

1. **Read:** REBRAND_SUMMARY.md (10 min)
2. **Plan:** Review execution timeline and phases (5 min)
3. **Prepare:** Create branch and gather materials (15 min)
4. **Execute:** Follow REBRAND_CHECKLIST.md (8-16 hours)
5. **Verify:** Run tests and validation (2-3 hours)
6. **Release:** Publish and announce (1-2 hours)

**Total: 11-19 hours to complete**

---

**Created:** March 16, 2026
**Scope:** Complete rebrand analysis from KairosUtamaIndonesia/kira-code to Kira Code
**Status:** Documentation complete, ready for execution

