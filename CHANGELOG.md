# SplitBill — Version History & Changelog

All notable changes and milestones for the SplitBill web application are documented in this file.

---

## [v2] - 2026-11-03

### Added
- **Mobile Keypad Optimization:** Added `inputmode="decimal"` on all item price, VAT, and SD inputs for instant calculator-style numeric pad on phones.
- **Safari Viewport Zoom Prevention:** Enforced 16px font-size rule on mobile inputs to eliminate iOS screen jumping.
- **Ergonomic Touch Targets:** Enlarged mobile tap areas for person sharing pills (36px min height) and item/person deletion buttons.

### Changed
- **Color System Overhaul:**
  - Introduced **Slate Periwinkle** (`#a5b4fc`) as the secondary accent for active states.
  - Refined person pills to a clean outline style (transparent background with colored border and text).
  - Reserved crimson red (`#e11d48`) strictly for section title dots and the Grand Total.
  - Card share totals switched to Slate Periwinkle to balance the visual hierarchy.
- **VAT & SD Controls:**
  - Switcher labels clarified from `৳ Flat` / `%` to `Amount` and `Rate (%)`.
  - In `Amount` mode, the redundant "Total:" preview line is hidden.
  - In `Rate (%)` mode, shows the computed taka amount preview.
- **Summary Section:**
  - Removed table view and view-switcher toggle; app now standardizes exclusively on responsive cards.
  - Summary header label updated from `FOOD SUBTOTAL` to `SUBTOTAL`.

### Preserved
- `index_v1.html` archived to preserve the initial v1.0 release snapshot.

---

## [v1.0] - 2026-10-27

### Initial Release
- **Core Functionality:**
  - Instant live recalculation on every keystroke/tap (no calculate button needed).
  - Add/remove people with custom inline names (starts with 3 by default, minimum 2).
  - Add/remove line items with item name, price in BDT (৳), and per-person sharing pills with "All" toggle.
  - Proportional tax distribution: VAT and Supplementary Duty (SD) allocated based on each person's food subtotal ratio.
  - Flat amount or percentage modes for VAT and SD.
  - Real-time Summary overview: Subtotal, VAT, SD, and Grand Total.
  - Split cards breakdown showing each person's food share, VAT share, SD share, and total.
- **Design & Architecture:**
  - Single self-contained HTML file (CSS + JS inline, zero frameworks, zero external dependencies).
  - Dark minimalist aesthetic: pure black (`#000000`), hairline borders, Instrument Serif headings, and Plus Jakarta Sans body font.
  - Hosted and deployed on GitHub Pages (`https://ahnafpatwary.github.io/splitbill`).
