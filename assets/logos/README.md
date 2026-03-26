# Iroko Labs — Logo Files

## Files included

| File | Use |
|---|---|
| `iroko-logo-dark.svg` | Primary lockup — dark / `#0f0d0a` backgrounds, hero section |
| `iroko-logo-light.svg` | Nav bar and any light / `#faf8f4` surfaces |
| `iroko-mark-dark.svg` | Standalone ring mark — dark backgrounds, social avatars |
| `iroko-mark-favicon.svg` | Favicon, og:image, app icon (solid gold fill) |

---

## Colours

| Token | Hex | Role |
|---|---|---|
| Gold | `#c9a84c` | Ring top arc, side branches, canopy nodes |
| Gold bright | `#e8c96a` | Optional hover / active state |
| Ink | `#0f0d0a` | Trunk, centre branch, centre node (dark bg: replaced by `#f5f2ec`) |
| Cream | `#f5f2ec` | Trunk + centre elements on dark backgrounds |
| Dim | `#7a7168` | "LABS" sub-label |

---

## Drop-in nav replacement

Replace the existing `.nav-logo` anchor in `index.html` with:

```html
<a href="/" class="nav-logo" style="display:flex;align-items:center;gap:0">
  <img src="/iroko-logo-light.svg" alt="Iroko Labs" height="44" width="auto"/>
</a>
```

Or inline the SVG directly for crisp rendering at all DPIs (recommended):

```html
<a href="/" class="nav-logo" aria-label="Iroko Labs">
  <!-- paste contents of iroko-logo-light.svg here -->
</a>
```

---

## Favicon (index.html `<head>`)

```html
<link rel="icon" type="image/svg+xml" href="/iroko-mark-favicon.svg">
<!-- PNG fallback for older browsers -->
<link rel="icon" type="image/png" sizes="32x32" href="/iroko-mark-favicon-32.png">
```

To generate PNG fallbacks, open `iroko-mark-favicon.svg` in Figma/Inkscape and export at 32×32 and 192×192.

---

## Clearspace rule

Minimum clearspace = **half the ring diameter** on all sides.
Never place any element closer than that to the mark.

## Minimum size

| Format | Minimum |
|---|---|
| Full lockup (mark + wordmark) | 120px wide |
| Mark only | 24px wide |
| Favicon | 16px (use solid gold fill version) |
