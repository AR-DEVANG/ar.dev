---
ai-generated: true
date: 2026-09-13
---
# Visual tokens

Live references inspected at desktop and 390 × 844: `https://sufiplugins.com/#top` and `https://www.apple.com/macbook-pro/`.

Sufi contributes a plain project index, separated chronological entries, project filtering, and incremental reveal. Its mobile navigation wraps and its statistics become a grid. Statistics and the activity heatmap are intentionally omitted because ar.dev has no equivalent release history.

Apple contributes large sans-serif headings, quiet navigation, rounded controls, image-led product explanation and selective dark sections. Browser inspection confirmed the SF Pro Text / Helvetica Neue sans-serif stack on the live page; use the operating system's own font stack rather than downloading Apple's fonts. The values below are ar.dev adaptations, not claimed exact measurements of either reference.

| Token | Light | Dark |
|---|---|---|
| Page | `#fafaf9` | `#111312` |
| Surface | `#ffffff` | `#1b1e1c` |
| Soft surface | `#f0f1ef` | `#252a27` |
| Text | `#1d1d1f` | `#f4f5f2` |
| Secondary text | `#65676b` | `#afb5af` |
| Hairline | `#dcdedb` | `#373e38` |
| Accent | `#356b50` | `#a8d4b6` |

- Layout: maximum 1184 px, 40 px desktop side allowance, 20 px mobile side allowance. Breakpoints at 1000, 700 and 370 px.
- Type: system sans, 17 px body / 1.55; hero `clamp(48px,6.7vw,96px)` with mobile override; section headings 36–62 px; ordinary project headings 32 px; 10–12 px metadata. Mono limited to schematic metadata.
- Containers: 26 px primary radius, 18–20 px secondary radius, pills 99 px; one-pixel borders. No lift on hover. The interface illustration has a restrained static shadow.
- Navigation: 70 px desktop, at least 64 px mobile; translucent local background and 22 px blur, with opaque-enough fallback color.
- Motion: 1 s hero arrival using `cubic-bezier(.2,.7,.2,1)`, opacity .6→1 and scale 1.025→1. No hidden text. Disable animations, transitions and smooth scrolling for either system reduced motion or local reduction.
- Reimagined: `#101714` surface, `#f4f7f3` headings, `#acb8ae` secondary text, `#e0eadd` active study control. The source and generated labels remain visible on images.
