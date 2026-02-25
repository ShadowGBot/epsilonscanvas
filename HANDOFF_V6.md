# V6 Handoff Pack — Investment UI Baseline

Project: `epsilonscanvas`  
Font baseline: **Plus Jakarta Sans**  
Style baseline: **Minimal, light-first, rounded (moderate)**

## 1) Approved Baseline

- Primary color: `#769FCD`
- Surface: `#D6E6F2`
- Background: `#F7FBFC`
- Accent soft: `#B9D7EA`
- Border: `#C8D9E8`
- Optional risk accent: `#BE5985`

Tokens and rationale are documented in `DESIGN_SYSTEM.md`.

## 2) Reference Prototypes

- Style Lab: `style-lab.html`
- Dashboard v3 (tabs/modal/charts): `investment-dashboard-v3.html`
- Playground v4 (component-focused): `investment-dashboard-v4.html`
- Production candidate v5: `investment-dashboard-v5.html`

## 3) Component Inventory (ETA build targets)

### Global Layout
- App shell: left nav + main content area
- Responsive collapse behavior for smaller screens

### Data Components
- Summary KPI cards (Regime, Confidence, Updated, P/L)
- Ticker movers table (sortable-ready)
- Chart cards (sparkline, allocation)
- Alpha vs Beta compare block
- Action checklist

### Interaction Components
- Tabs (Pulse / Alpha-Beta / News)
- Modal (rebalance settings)
- Filter bar (date/session/ticker)
- Quick actions panel

### State Components
- Loading skeleton
- Empty state (clear next step CTA)
- Error state (retry CTA)

## 4) Behavior + Acceptance Criteria

### Navigation
- Switching nav item swaps active view without full reload
- Active nav item has visible selected state

### Table
- Columns remain readable on mobile via horizontal scroll
- Positive/negative deltas clearly color-coded

### Modal
- Opens via trigger button
- Closes via close button and overlay click
- Focus should be trapped in production implementation

### States
- Every data module must define loading/empty/error/success
- Error state must include human-readable message + retry action

### Accessibility (required for production)
- Keyboard tab order and focus rings on controls
- ARIA labels for modal, tabs, interactive controls
- Color contrast checks for text on badges/buttons

## 5) Implementation Priority

### P1 (ship first)
- App shell, summary cards, ticker table, filter bar
- Loading/empty/error states
- Typography + token integration

### P2
- Tabs + Alpha/Beta block + chart cards
- Modal interactions

### P3
- Polished micro-interactions
- Export/share actions
- Advanced sorting/filter persistence

## 6) Reuse Across Other Sites

This system is reusable for different project types by swapping domain modules:
- Replace “Ticker table” with domain-specific table/list
- Keep same shell/cards/forms/states/tokens
- Retain typography + spacing standard for consistent family feel

## 7) Final Recommendation

Yes — we now have enough core system pieces to design and build different sites with consistency.
What’s left is mainly **project-specific content architecture and domain components**, not base UI foundations.
