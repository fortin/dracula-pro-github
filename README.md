# Dracula Pro for GitHub (Cascadea / User CSS)

A **Dracula Pro–inspired GitHub theme** implemented as **pure CSS**, designed for use with **Cascadea** (Safari), **Stylus** (Chrome / Firefox), and compatible user-style tools on other browsers.

This theme adapts GitHub’s UI to the Dracula Pro palette while respecting GitHub’s existing CSS variable system and branding.

It also includes an **optional, subtle Dracula Pro–styled Octocat header logo** (with tiny fangs), designed as an easter egg rather than a replacement.

---

## Features

- 🎨 **Dracula Pro color palette**
  - Deeper base background
  - Refined surface hierarchy
  - Pro accent purple
  - Tuned borders, buttons, and hover states
- 🔗 **Readable link styling**
  - Clear contrast
  - Consistent with classic Dracula readability
- 🧛 **Optional Dracula Pro Octocat**
  - Preserves GitHub silhouette
  - Subtle white fangs
  - No layout or click behavior changes
- 🧼 **Pure CSS**
  - No JavaScript
  - No DOM mutation
  - Stable across GitHub updates

---

## Screenshots

*(Optional — add screenshots here if contributing upstream)*

---

## Installation (Safari via Cascadea)

### 1. Install Cascadea
Cascadea is a user stylesheet manager for Safari.

- Website: https://cascadea.app
- Available on the Mac App Store

### 2. Create a New Style
1. Open **Cascadea**
2. Click **“+” → New Style**
3. Set **Applies to**:  github.com

### 3. Paste the CSS
1. Open the provided CSS file in this repository
2. Copy **all contents**
3. Paste into the Cascadea editor
4. Save the style

### 4. Reload GitHub
Refresh any open GitHub tabs. The theme should apply immediately.

---

## Installation (Other Browsers)

This CSS also works with:
- **Stylus** (Chrome / Firefox)―though you are probably better off using the [official Stylus theme](https://draculatheme.com/github) on those browsers.
- **Firefox userContent.css**

When using Stylus:
- Remove any `@-moz-document` wrappers if present
- Scope the style to `github.com`

---

## Configuration

This theme is intentionally **static** (no runtime toggles).

If you want to customize it:
- Adjust CSS variables near the top of the file
- Modify accent colors (`--color-accent-*`)
- Disable the Octocat modification by removing the final logo block

All changes are localized and safe.

---

## Dracula Pro Octocat (Optional)

The theme includes an optional header logo variant:

- GitHub Octocat silhouette (unchanged)
- Dracula Pro accent purple
- Two small white fangs
- Slight inward slant for a subtle “Dracula smile”

This is implemented via CSS using a replacement SVG injected with `::before`.

To disable it, remove or comment out the section labeled:

```css
/* GitHub header logo — Dracula Pro Octocat */
