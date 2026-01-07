# TODO

## Priority: High

- [ ] **FIX SLIDE ALIGNMENT** - v0.4.1 "align to left" swapped positions on several slides
  - Slides 05, 08, 14 (and possibly others) have left/right positions reversed
  - What was on the left is now on the right, and vice versa
  - Compare each slide against deployed version at jan26-five.vercel.app to identify issues
  - Swap content back to original positions

## Priority: Medium

- [ ] Add smooth scroll navigation between slides
- [ ] Add keyboard navigation (arrow keys)
- [ ] Consider adding slide indicators/progress bar
- [ ] Mobile menu for navigation (hamburger)

## Priority: Low

- [ ] HUD button styling options (explore color/outline variations)
- [ ] Add print styles for PDF export
- [ ] Add meta tags for SEO/sharing
- [ ] Add favicon
- [ ] Performance optimization (lazy load images)

---

## Completed

- [x] Initial HTML structure (2025-01-05)
- [x] Sticky header with blur effect (2025-01-05)
- [x] Responsive breakpoints (2025-01-05)
- [x] All 20 slides content (2026-01-06)
- [x] Git repo setup and GitHub connection (2025-01-05)
- [x] Dropdown navigation to all slides (2025-01-05)
- [x] OS HUD button connected to pre-viz (2026-01-06)
- [x] Slide anchor IDs for navigation (2025-01-05)
- [x] Agenda slide added (slide 2) with 10 topics (2026-01-06)
- [x] Title updated: "Working Session" (CEO removed) (2026-01-06)
- [x] All placeholder images complete (2026-01-06)
- [x] Flywheel image: cleanflywheel.png (2026-01-06)
- [x] **Proof slide pill fix** - "The Ask" pill now uses `<span onclick>` instead of nested `<a>` (2026-01-06)
  - Fixed: Tiles display side-by-side correctly
  - Fixed: Both CYLNDR card link and "The Ask" pill link work independently

---

## Notes

### Header Navigation (Upcoming)
```
Nav structure to implement:
- Logo (left)
- Nav links (center or right)
- OS HUD button (right)
```

### OS HUD Integration
- ~~Dummy button added with placeholder alert~~
- [x] Connected to https://brandstudiosai-pre-viz.vercel.app/ (2026-01-06)
- Look for: `class="nav-hud-btn"` in index.html

### Session 2026-01-06 Notes
- The nested `<a>` tag issue caused browsers to break CYLNDR card structure
- Solution: Changed inner pill from `<a>` to `<span onclick="window.open(...)"`
- This is the ONLY change from v0.4.1 that should be kept
