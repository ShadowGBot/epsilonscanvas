# Epsilon Design System v1 (Default)

Owner: Epsilon 🦦  
Context owner: Kanta / KingK

## Default Rules

1. **Mode:** minimal (default)
2. **Theme:** light-first (dark only when requested)
3. **Buttons:** rounded, but not pill-heavy

---

## Visual Direction

- Mood targets: calm, premium, sharp, playful (context-dependent)
- Component feel options: minimal / glassy / fintech
- Baseline for unspecified work: **minimal + light**

## Color Palettes

### Primary blue family
- `#F7FBFC` (page bg)
- `#D6E6F2` (surface)
- `#B9D7EA` (accent soft)
- `#769FCD` (primary action)

### Secondary pink family
- `#FFEDFA`
- `#FFB8E0`
- `#EC7FA9`
- `#BE5985`

Usage: blue family is default for product UI; pink is optional thematic/accent palette.

## Typography

- Primary: **Inter** (default)
- Fallback: `ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial`
- Style target: professional, clean, high readability

Scale baseline:
- Display: 32/40
- H1: 28/36
- H2: 22/30
- H3: 18/26
- Body: 15/24
- Small: 13/20

## Radius

- Card/input: `12px`
- Button: `10px`
- Chips/badges: `999px` only when semantically needed

## Shadow

Subtle layered shadows (light mode):
- `shadow-sm`: `0 1px 2px rgba(16,24,40,.06)`
- `shadow-md`: `0 6px 16px rgba(16,24,40,.08)`
- `shadow-lg`: `0 12px 28px rgba(16,24,40,.12)`

## Spacing & Density

- 8px grid
- Density: balanced
- Page gutter: 24–32px desktop, 16px mobile
- Card padding: 16–20px
- Section spacing: 24–40px

## Component Defaults

- Tables: compact rows but clear separators
- Forms: clear labels + helper text; never placeholder-only
- States always included: empty, loading, error, success
- Focus rings required on interactive controls

## Delivery Standard per feature

1. UX packet (flow/state/acceptance criteria)
2. React+TS+Tailwind prototype
3. UI audit vs implemented screen
4. ETA-ready handoff checklist

## References

- Minimal inspiration: https://www.dstudio.agency/
- Fintech inspiration: https://awsmd.com/
- Investment UX reference: https://www.google.com/finance/quote/GOOG:NASDAQ
