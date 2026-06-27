# Air Fryer Meal Prep Visual Style Guide

## Core Palette

| Role | Hex | Usage |
| --- | --- | --- |
| Medium Brown | `#c99b38` | Warm highlights, secondary accents, grounding elements |
| Light Brown | `#eddca5` | Soft backgrounds, muted badges, gentle highlight areas |
| Medium Teal | `#00b0be` | Primary accent, progress, active states, important highlights |
| Light Teal | `#8fd7d7` | Soft accent backgrounds, gradients, supporting visual areas |

## Theme Direction

Use a clean, practical dashboard style. The site should feel fresh, calm, and structured, with teal for clarity and action, and brown/gold for warmth.

Avoid heavy brown-only layouts, purple gradients, decorative blobs, or overly playful styling. Keep the page polished, clear, and easy to scan.

## CSS Tokens

Use these custom properties as the base for future pages:

```css
:root {
  color-scheme: light;
  --bg: #f7f4e8;
  --bg-soft: #fff9df;
  --surface: rgba(255, 252, 236, 0.84);
  --surface-strong: #fffaf0;
  --border: rgba(201, 155, 56, 0.22);
  --border-strong: rgba(0, 176, 190, 0.28);
  --text: #15181a;
  --muted: #5f6e70;
  --accent: #00b0be;
  --accent-strong: #007d87;
  --accent-soft: rgba(0, 176, 190, 0.14);
  --success: #008f9a;
  --warning: #c99b38;
  --track-low: #eddca5;
  --track-high: linear-gradient(90deg, #c99b38, #00b0be);
}

[data-theme="dark"] {
  color-scheme: dark;
  --bg: #111b1d;
  --bg-soft: #142528;
  --surface: rgba(18, 34, 37, 0.88);
  --surface-strong: #172e31;
  --border: rgba(143, 215, 215, 0.18);
  --border-strong: rgba(237, 220, 165, 0.26);
  --text: #f8f3e4;
  --muted: #bfd5d4;
  --accent: #8fd7d7;
  --accent-strong: #b9eeee;
  --accent-soft: rgba(143, 215, 215, 0.18);
  --success: #00b0be;
  --warning: #eddca5;
  --track-low: #24464a;
  --track-high: linear-gradient(90deg, #00b0be, #eddca5);
}
```

## Layout Style

Use full-page, app-like layouts rather than a marketing landing page. Keep content organized in clear sections with compact cards, soft borders, and subtle depth.

Cards should use a maximum border radius of `28px` only for large containers and `14px-18px` for compact items. Avoid nested cards where possible.

## Component Rules

- Primary accents: use medium teal `#00b0be`.
- Secondary accents: use medium brown `#c99b38`.
- Soft backgrounds: use light brown `#eddca5` or light teal `#8fd7d7` at low opacity.
- Progress bars: use a brown-to-teal gradient in light mode.
- Badges: use soft fills with strong text, not solid saturated backgrounds.
- Borders: keep them translucent and warm in light mode, teal-tinted in dark mode.
- Shadows: use low-opacity teal or brown shadows only.

## Typography

Use Inter or a similar modern sans-serif. Headings should be confident and compact with tight line height. Body copy should be direct, calm, and practical.

Avoid oversized decorative type inside dashboards, cards, lists, and controls.

## Backgrounds

Use pale cream backgrounds with light teal and light brown directional gradients. Keep the background quiet enough that meal cards, stats, and lists remain the focus.

Do not use decorative orbs, bokeh, or heavy single-color gradient backgrounds.

## Tone

The content voice should be useful, concise, and reassuring. Prefer practical labels like `Fast prep`, `Office-friendly`, `Low cleanup`, and `Goal progress`.
