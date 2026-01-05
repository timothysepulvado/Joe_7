# Project Structure

Quick reference for navigating the codebase.

## Files

```
Joe_7/
├── index.html      # Main presentation file
├── CHANGELOG.md    # Version history and changes
├── TODO.md         # Task tracking
├── STRUCTURE.md    # This file - project map
└── .gitignore      # Git ignore rules
```

## index.html Overview

### CSS Variables (`:root`)
Location: `<style>` block, lines ~5-10

| Variable        | Value      | Usage                    |
|-----------------|------------|--------------------------|
| `--navy`        | `#0f1419`  | Primary dark             |
| `--navy-light`  | `#1a2028`  | Card backgrounds         |
| `--orange`      | `#e85d2d`  | Accent/brand color       |
| `--cream`       | `#fafaf8`  | Page background          |
| `--warm-white`  | `#fff`     | Card backgrounds         |
| `--text`        | `#2c3038`  | Body text                |
| `--text-light`  | `#5a6270`  | Secondary text           |
| `--green`       | `#10b981`  | Success/positive         |
| `--blue`        | `#5b8fd9`  | Info/accent              |
| `--coral`       | `#e07a5f`  | Warm accent              |
| `--serif`       | Playfair   | Headlines                |
| `--sans`        | Inter      | Body text                |

### Key CSS Classes

| Class              | Purpose                              |
|--------------------|--------------------------------------|
| `.slide`           | Full-height section container        |
| `.slide-inner`     | Max-width content wrapper            |
| `.display`         | Large serif headlines                |
| `.headline`        | Medium serif headlines               |
| `.body-lg`         | Large body text                      |
| `.theme-label`     | Section number labels                |
| `.split`           | Two-column grid layout               |
| `.category-cards`  | Three-column card grid               |
| `.dimension-cards` | Three-column dark cards              |
| `.dark-card`       | Navy gradient card                   |
| `.fidelity-card`   | Brand fidelity score card            |

### Slide Index

| #  | ID/Section | Title                              |
|----|------------|------------------------------------|
| 1  | Title      | BrandStudios.AI × Cheil            |
| 2  | 01         | The Market Problem: Systemic Drift |
| 3  | 02         | The Opportunity Gap                |
| 4  | 03         | HoldCo AI Platform Comparison      |
| 5  | 04         | The Difference That Matters        |
| 6  | 05         | One Connected Creative Brain       |
| 7  | 06         | BrandStudios.AI Platform           |
| 8  | 07         | Three Dimensions                   |
| 9  | 08         | Five Pillars                       |
| 10 | 09         | Brand Fidelity                     |
| 11 | 10         | Proof                              |
| 12 | 11         | Performance Signals                |
| 13 | 12         | How Cheil Wins                     |
| 14 | 13         | Market Opportunity                 |
| 15 | 14         | Why Timing Matters                 |
| 16 | 15         | Cannes: The Narrative Shift        |
| 17 | 16         | Defensibility                      |
| 18 | Next Steps | The Commercial Flywheel            |
| 19 | Close      | Human Intelligence, Amplified      |
| 20 | Footer     | Copyright bar                      |

### Responsive Breakpoints

| Breakpoint | Target         | Key Changes                    |
|------------|----------------|--------------------------------|
| > 1024px   | Desktop        | Full layouts                   |
| ≤ 1024px   | Tablet         | Single column grids            |
| ≤ 768px    | Mobile         | Reduced padding, 2-col pillars |

## Quick Edit Guide

### To change brand colors:
Edit CSS variables in `:root` section

### To add a new slide:
1. Copy existing `<section class="slide">` block
2. Update slide number in `.slide-footer`
3. Update theme-label number

### To modify header:
Edit the `<nav>` element near top of `<body>`

### To add navigation:
Inside `<nav>`, add after `.logo` div
