---
name: Apple-Inspired Design System
colors:
  primary: "#0071E3"
  accent: "#1D1D1F"
  neutral: "#F5F5F7"
typography:
  h1:
    fontFamily: "-apple-system, BlinkMacSystemFont, 'SF Pro Display', 'Helvetica Neue', sans-serif"
    fontSize: "3.5rem"
  h2:
    fontFamily: "-apple-system, BlinkMacSystemFont, 'SF Pro Display', 'Helvetica Neue', sans-serif"
    fontSize: "2.5rem"
  h3:
    fontFamily: "-apple-system, BlinkMacSystemFont, 'SF Pro Text', 'Helvetica Neue', sans-serif"
    fontSize: "1.5rem"
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, 'SF Pro Text', 'Helvetica Neue', sans-serif"
    fontSize: "1.0625rem"
  caption:
    fontFamily: "-apple-system, BlinkMacSystemFont, 'SF Pro Text', 'Helvetica Neue', sans-serif"
    fontSize: "0.875rem"
spacing:
  xs: "8px"
  sm: "12px"
  md: "22px"
  lg: "40px"
  xl: "80px"
rounded:
  sm: "8px"
  md: "12px"
  lg: "18px"
  pill: "980px"
---

## Overview

An Apple-inspired design system built on clarity, deference, and depth. The
visual language leans on generous whitespace, a near-black ink (`#1D1D1F`) on
soft off-white surfaces (`#F5F5F7`), and a single confident blue
(`#0071E3`) reserved for actions and links. Type does the heavy lifting:
large, tightly-tracked SF-style display headings paired with calm, legible
body copy.

## Color

- **Primary `--color-primary` (`#0071E3`)** — Apple's signature interactive
  blue. Use it only for primary buttons, links, and key calls-to-action.
  Never use it for large background fills.
- **Accent `--color-accent` (`#1D1D1F`)** — the near-black "ink" used for all
  headings and body text, and for high-contrast hero sections. Not pure black,
  which feels harsh on screen.
- **Neutral `--color-neutral` (`#F5F5F7`)** — the soft, slightly warm grey that
  defines Apple's section backgrounds and cards, separating content without
  hard borders.

Maintain WCAG AA: ink on neutral exceeds 4.5:1; white text only ever sits on
the ink or on the saturated blue.

## Typography

The system relies on the platform San Francisco stack with graceful fallbacks.
Headings (`--type-h1` / `--type-h2`) are large, semibold, and tightly tracked
(`letter-spacing: -0.02em`) for that crisp Apple display feel. Body text stays
relaxed at `1.0625rem` with a `1.5` line-height for comfortable reading.

- `--type-h1-font-size`: hero statements ("Think different.")
- `--type-h2-font-size`: section headlines
- `--type-h3-font-size`: card and feature titles
- `--type-body-font-size`: paragraphs and UI text
- `--type-caption-font-size`: legal, footnotes, metadata

## Spacing

A roomy scale that favors breathing room over density. Sections typically use
`--spacing-xl` (80px) vertical rhythm, content blocks use `--spacing-lg`, and
inline element gaps use `--spacing-sm`/`--spacing-xs`.

## Radius

Soft, modern corners. Cards and surfaces use `--radius-md`/`--radius-lg`;
buttons use `--radius-pill` (980px) for Apple's fully-rounded capsule buttons.

## Usage Notes

- Buttons: blue background, white text, `--radius-pill`, generous horizontal
  padding (`--spacing-md`).
- Links: `--color-primary`, no underline by default, underline on hover.
- Sections alternate between white and `--color-neutral` backgrounds.
- Reference the injected custom properties (`--color-*`, `--type-*`,
  `--spacing-*`, `--radius-*`) — never hard-code these hex values again.
