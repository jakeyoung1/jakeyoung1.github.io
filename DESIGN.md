# DESIGN.md — "Scorecard"

Vintage printed stat sheet: cream paper, green ink, red rubber stamp. Register: brand.

## Color (OKLCH)

| Token | Value | Use |
|---|---|---|
| `--paper` | `oklch(95.8% 0.014 92)` | page background |
| `--paper-deep` | `oklch(92.6% 0.022 95)` | table header tint |
| `--ink` | `oklch(24% 0.045 155)` | primary text, heavy borders |
| `--ink-soft` | `oklch(38% 0.04 155)` | secondary text |
| `--ink-faint` | `oklch(52% 0.03 155)` | labels, legends |
| `--stamp` | `oklch(49% 0.185 28)` | links, section numbers, stamp, accents only |

Strategy: Committed (green ink carries the whole surface; red stays under 10%).

## Type

- Libre Franklin: 900 for display/headings/stat values, 400/500 body. Uppercase display.
- Spline Sans Mono: 400–600 for labels, legends, nav, table headers, tool lists. Uppercase, letter-spaced 0.08–0.18em.
- Body 1.0625rem / 1.55. Headings clamp() fluid.

## Structure rules

- Tables are first-class content (`.statline`, `.skills-table`): 2px ink outer border, 1px rule cells, tinted header row.
- Double rules (`border: 3px double`) mark document-level boundaries (masthead label, nav, colophon).
- Single 1px rules separate sections; faint rules separate report rows.
- No cards, no shadows, no gradients, no border-radius (except 3px on the stamp).
- The stamp: red 2.5px border, mono caps, rotate(-4deg), red 8% background.

## Voice

Scorekeeping register: "Season line", "Scouting reports", "Service record", "Contact the front office". Every number real. No em dashes.
