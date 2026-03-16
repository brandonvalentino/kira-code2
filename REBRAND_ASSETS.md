# Vibe Kanban → Kira Code Rebrand: Asset Inventory

## Summary
Found **17 logo/favicon/image assets** and **40+ code references** that need rebrand updates.

---

## 🎨 Image Assets to Rename/Replace

### Logos (Primary Branding)
**Location:** `packages/public/`

| Current Filename | Type | Purpose | Action |
|---|---|---|---|
| `vibe-kanban-logo.svg` | SVG | Light mode logo (landing/UI) | **REPLACE** with `kira-code-logo.svg` |
| `vibe-kanban-logo-dark.svg` | SVG | Dark mode logo (landing/UI) | **REPLACE** with `kira-code-logo-dark.svg` |

**Files that reference these:**
- `packages/web-core/src/pages/migrate/MigratePage.tsx` (lines 49-50)
- `packages/web-core/src/features/onboarding/ui/OnboardingSignInPage.tsx` (lines 99-100)
- `packages/web-core/src/features/onboarding/ui/LandingPage.tsx` (lines 179-180)
- `packages/remote-web/src/shared/components/BrandLogo.tsx` (lines 13, 16)

### Favicons
**Location:** `packages/public/`

| Current Filename | Type | Purpose | Action |
|---|---|---|---|
| `favicon-vk-light.svg` | SVG | Light mode favicon | **REPLACE** with `favicon-kc-light.svg` (or keep simpler naming) |
| `favicon-vk-dark.svg` | SVG | Dark mode favicon | **REPLACE** with `favicon-kc-dark.svg` |
| `favicon-vk-light-maskable.svg` | SVG | Maskable icon for home screen | **REPLACE** with `favicon-kc-light-maskable.svg` |

**Files that reference these:**
- `packages/local-web/index.html` (lines 6-7)
- `packages/public/site.webmanifest` (lines 4-13)

### Screenshots/Guides
**Location:** `packages/public/`

| Current Filename | Type | Purpose | Action |
|---|---|---|---|
| `vibe-kanban-screenshot-overview.png` | PNG | Marketing/guide screenshot | **REPLACE** with new screenshots |
| `vibe-kanban-screenshot-workspace.png` | PNG | Marketing/guide screenshot | **REPLACE** with new screenshots |

### Other Assets (Keep as-is)
- `apple-touch-icon.png` - Generic, can keep
- `favicon.png` - Generic fallback, can keep
- `logo_light.png` - Generic, can keep
- `beta-workspaces-preview.png` - Generic, can keep
- `guide-images/*.png` - Product guide images, no branding

---

## 📝 Code References to Update

### Configuration & Manifest Files

1. **`packages/public/site.webmanifest`** (JSON metadata)
   - Line 1: `"name": "Vibe Kanban"` → `"Kira Code"`
   - Line 2: `"short_name": "VK"` → `"KC"` (or `"Kira Code"`)
   - Lines 4-13: Update favicon paths from `favicon-vk-*` → `favicon-kc-*`

### Package Configuration

2. **`package.json`** (root)
   - Line 2: `"name": "vibe-kanban"` → `"kira-code"` (affects NPM publishing)
   - Line 6: `"vibe-kanban": "npx-cli/bin/cli.js"` → `"kira-code"`

3. **`npx-cli/package.json`**
   - Line 2: `"name": "vibe-kanban"` → `"kira-code"`
   - Line 7: `"vibe-kanban": "bin/cli.js"` → `"kira-code"`
   - Line 17: URL `https://github.com/KairosUtamaIndonesia/kira-code` → `kira-code` (or new URL)
   - Line 23: `"NPX wrapper around vibe-kanban..."` → update description

### HTML Entry Points

4. **`packages/local-web/index.html`** (lines 6-8)
   - Favicon references: `favicon-vk-light.svg` → `favicon-kc-light.svg`
   - Favicon references: `favicon-vk-dark.svg` → `favicon-kc-dark.svg`

### React/TypeScript Components

5. **`packages/web-core/src/pages/migrate/MigratePage.tsx`** (lines 49-50)
   ```
   '/vibe-kanban-logo-dark.svg' → '/kira-code-logo-dark.svg'
   '/vibe-kanban-logo.svg' → '/kira-code-logo.svg'
   ```

6. **`packages/web-core/src/features/onboarding/ui/OnboardingSignInPage.tsx`** (lines 99-100)
   ```
   '/vibe-kanban-logo-dark.svg' → '/kira-code-logo-dark.svg'
   '/vibe-kanban-logo.svg' → '/kira-code-logo.svg'
   ```

7. **`packages/web-core/src/features/onboarding/ui/LandingPage.tsx`** (lines 179-180)
   ```
   '/vibe-kanban-logo-dark.svg' → '/kira-code-logo-dark.svg'
   '/vibe-kanban-logo.svg' → '/kira-code-logo.svg'
   ```

8. **`packages/remote-web/src/shared/components/BrandLogo.tsx`** (lines 13, 16)
   ```
   srcSet="/vibe-kanban-logo-dark.svg" → "/kira-code-logo-dark.svg"
   src="/vibe-kanban-logo.svg" → "/kira-code-logo.svg"
   alt="Vibe Kanban" → "Kira Code"
   ```

### GitHub/Repository References

9. **`packages/ui/src/components/AppBar.tsx`** (line 392)
   ```
   href="https://github.com/KairosUtamaIndonesia/kira-code" → new repo URL
   ```

10. **`packages/web-core/src/features/onboarding/ui/LandingPage.tsx`** (line 117)
    ```
    href: 'https://github.com/KairosUtamaIndonesia/kira-code' → new repo URL
    ```

11. **`packages/web-core/src/shared/dialogs/global/ReleaseNotesDialog.tsx`** (line 15)
    ```
    'https://github.com/KairosUtamaIndonesia/kira-code/releases' → new URL
    ```

### CLI & Runtime References

12. **`npx-cli/src/cli.ts`** (multiple lines)
    - Line 209: `npx vibe-kanban@latest` → `npx kira-code@latest`
    - Line 255: `Starting vibe-kanban desktop...` → `Starting Kira Code...`
    - Line 275: `Starting vibe-kanban v${CLI_VERSION}` → `Starting Kira Code...`
    - Line 310: `cac("vibe-kanban")` → `cac("kira-code")`
    - Line 313: `"Launch the local vibe-kanban app"` → `"Launch the local Kira Code app"`
    - Line 217, 234: Command references to `"vibe-kanban-mcp"`, `"vibe-kanban-review"` → update names

13. **`npx-cli/src/desktop.ts`** (line 238)
    - Binary name reference: `'vibe-kanban'` → `'kira-code'`

14. **`npx-cli/src/download.ts`** (lines 10, 202)
    ```
    CACHE_DIR = path.join(os.homedir(), '.vibe-kanban', 'bin')
    → path.join(os.homedir(), '.kira-code', 'bin')
    
    '.vibe-kanban' → '.kira-code'
    ```

### Build Configuration

15. **`packages/local-web/vite.config.ts`** (line 111)
    ```
    sentryVitePlugin({ org: 'bloop-ai', project: 'vibe-kanban' })
    → sentryVitePlugin({ org: 'bloop-ai', project: 'kira-code' })
    ```

### Cryptographic/Protocol Constants

16. **`packages/web-core/src/shared/lib/relayPake.ts`** (lines 5-6)
    ```
    SPAKE2_CLIENT_ID = 'vibe-kanban-browser' → 'kira-code-browser'
    SPAKE2_SERVER_ID = 'vibe-kanban-server' → 'kira-code-server'
    ```
    ⚠️ **NOTE:** This is protocol level. Changing may break existing relay connections. Consider backwards compatibility.

### PR/Commit Metadata

17. **`packages/web-core/src/shared/dialogs/command-bar/CreatePRDialog.tsx`** (line 51)
    ```
    PR_TITLE_SUFFIX = ' (vibe-kanban)' → ' (kira-code)'
    ```

### Workspace Directory Names

18. **Multiple `.json` localization files** (settings translations)
    - `packages/web-core/src/i18n/locales/*/settings.json`
    - References to `.vibe-kanban-workspaces` directory:
      - Line 160-163 in: `en/settings.json`, `zh-Hans/settings.json`, `ko/settings.json`, `zh-Hant/settings.json`, `es/settings.json`, `fr/settings.json`
    - **Action:** Replace `.vibe-kanban-workspaces` → `.kira-code-workspaces` in all locale files

### Documentation

19. **`npx-cli/README.md`** (multiple lines)
    - Branding references throughout
    - Update all instances of "Vibe Kanban" → "Kira Code"

20. **Root `README.md`** (multiple lines)
    - Line 6: Image reference `packages/public/vibe-kanban-logo.svg`
    - Lines 28, 60, 126-144: All environment variables and references

21. **`crates/remote/README.md`** (line 3, 56, etc.)
    - Update documentation for remote API

---

## 🔧 Recommended Rebrand Workflow

### Phase 1: Asset Replacement
1. Create new SVG logos: `kira-code-logo.svg`, `kira-code-logo-dark.svg`
2. Create new favicon SVG files: `favicon-kc-light.svg`, `favicon-kc-dark.svg`, `favicon-kc-light-maskable.svg`
3. Create new screenshots (or remove if deprecated)
4. Delete old `vibe-kanban-*.svg`, `favicon-vk-*.svg`, `vibe-kanban-screenshot-*.png`

### Phase 2: Configuration Updates
1. Update `site.webmanifest` (JSON + favicon references)
2. Update `package.json` files (root, npx-cli) - affects NPM publishing
3. Update HTML entry points (index.html)

### Phase 3: Code Updates
1. Update all component imports (BrandLogo.tsx, OnboardingSignInPage.tsx, etc.)
2. Update all image path references
3. Update GitHub URLs
4. Update CLI command names and output messages
5. Update Sentry project name
6. Update SPAKE2 identifiers (⚠️ may have protocol implications)

### Phase 4: Localization & Docs
1. Update workspace directory references in all i18n JSON files
2. Update README files
3. Update user-facing strings

### Phase 5: Testing
- Run `pnpm run format` and `pnpm run lint`
- Test local-web and remote-web builds
- Verify favicon display in different browsers
- Check relay protocol compatibility

---

## 📊 File Change Summary

| Category | Count |
|----------|-------|
| Image assets to replace | 5 |
| Favicon files to replace | 3 |
| Screenshots to replace | 2 |
| Configuration files | 3 |
| React components | 4 |
| CLI/NPX files | 3 |
| Localization files | 6 |
| Documentation files | 3 |
| Miscellaneous references | 15+ |
| **TOTAL FILES TO MODIFY** | **~40+** |

---

## ⚠️ Critical Notes

1. **NPM Publishing:** Changing `package.json` name affects NPM distribution. Ensure new name `kira-code` is available.
2. **Protocol Breaking Change:** SPAKE2 identifiers are cryptographic. Changing these may break existing relay connections. Consider version migration.
3. **GitHub URLs:** Ensure new GitHub repo exists and is publicly accessible before updating URLs.
4. **Workspace Migration:** Users with existing `.vibe-kanban-workspaces` directories won't automatically migrate to `.kira-code-workspaces`. Consider migration logic.
5. **Icon Caching:** Favicons are aggressively cached. Consider cache-busting strategies (query params, hash versioning).
