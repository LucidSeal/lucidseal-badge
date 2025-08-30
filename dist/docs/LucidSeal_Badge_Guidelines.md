# LucidSeal Badge — Usage Guidelines (v1)

The LucidSeal badge signals digital trust. Keep usage simple and consistent.

## Variants
- **Dark (primary):** navy stroke `#1d2d44` on light backgrounds. File: `badge-dark.svg`
- **Light (inverse):** white stroke `#ffffff` on dark backgrounds. File: `badge-light.svg`
- **Favicon/Icon:** uses `currentColor` so it inherits the surrounding text color. File: `badge-favicon.svg`
- **SVG Set (symbols):** `lucidseal-badge-set.svg` contains `lucidseal-badge-dark` and `lucidseal-badge-light` symbols for `<use>` embedding.

## Clear Space
Reserve clear space around the badge equal to the height of the badge’s checkmark (≈ one third of total height). No other graphics or text within this area.

## Minimum Size
- Digital: 20px height minimum.
- Print: 7mm height minimum.

## Color
- Primary stroke color: `#1d2d44` (navy).
- Inverse stroke color: `#FFFFFF` (white).
- Do **not** apply gradients, shadows, or outlines.

## Backgrounds
- Approved: white, off‑white, very light neutrals for dark variant; navy/near‑black for inverse.
- Avoid: busy images, low‑contrast colors.

## Don’ts
- Don’t recolor outside the palette.
- Don’t distort, stretch, or rotate.
- Don’t place over complex imagery.
- Don’t add drop shadows or effects.

## Pairing with Wordmark
The badge is icon‑only. Pair with the “LucidSeal” wordmark set in your site’s UI font (recommended: system‑ui stack). Typical lockup:
```
[badge] LucidSeal
```
Maintain at least the badge’s clear space between icon and text. Wordmark height should be **1.0–1.25×** the badge height.

## Embedding Examples

**Inline `<img>`:**
```html
<img src="/assets/badge-dark.svg" alt="LucidSeal badge" width="48" height="48">
```

**On dark header (inverse):**
```html
<header style="background:#0f172a">
  <img src="/assets/badge-light.svg" alt="LucidSeal badge" width="48" height="48">
</header>
```

**Symbol `<use>` (from the set):**
```html
<!-- include the symbol set once, e.g., via <object> or inline server-side -->
<object type="image/svg+xml" data="/assets/lucidseal-badge-set.svg"></object>

<!-- reference the symbol -->
<svg width="48" height="48" aria-label="LucidSeal badge">
  <use href="#lucidseal-badge-dark"></use>
</svg>
```

**Favicon (SVG):**
```html
<link rel="icon" type="image/svg+xml" href="/assets/badge-favicon.svg">
```

## Versioning
Name files with semantic versions when updated, e.g., `badge-dark.v1.1.svg`. Keep a CHANGELOG for visual changes.

---

© LucidSeal. Use the badge to indicate participation/commitment to the LucidSeal principles. Do not imply certification unless explicitly granted.