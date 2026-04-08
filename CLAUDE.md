# Korean-Style Presentation Template — LG Field Service Slides

## What This Is

A reusable slide generation system for LG Electronics leadership presentations. The formatting follows Korean corporate presentation conventions — clean, data-dense, color-coded, with a strict separation between **Review** (what happened) and **Strategy** (what we're doing about it).

Daniel regularly needs slides built or reformatted in this style. Anyone giving him a deck to "run magic on" gets it converted to this format. This is plug-and-play — read the rules, apply them, done.

---

## The Korean Slide Philosophy

Korean leadership presentations have distinct conventions that differ from typical Western corporate decks:

### Review vs Strategy — They Are NOT the Same

| | Review (Left Column) | Strategy (Right Column) |
|---|---|---|
| **Purpose** | What happened. Where things stand. | What we are doing about it. The plan. |
| **Tone** | Factual, data-driven, backward-looking | Forward-looking, action-oriented |
| **Content** | Metrics, trends, deltas, specific numbers | Frameworks, approaches, targets, methodology |
| **NEVER do** | Put strategy language in review | Put specific ASC names or "what's wrong" in strategy |

**Critical rule:** Strategy sections describe THE STRATEGY — not which accounts are bad. Leadership doesn't want "Appliance Medic is at 59.8D" in strategy. They want "we rank by impact score, apply REPAIR, and cycle the list." The strategy should work regardless of which specific accounts are underperforming.

### Data Presentation Rules

1. **Green (#228B22) = Good / Improving** — RTAT going down, metrics improving, targets met
2. **Red (#CC0000) = Bad / Worsening** — RTAT going up, metrics declining, targets missed
3. **Black (#000000) = Neutral / Baseline** — Reference data, labels, descriptions
4. **Gray (#999999) = Secondary info** — Subtitles, supporting context
5. **White (#FFFFFF) = Table headers on dark background**

### Color Logic for RTAT Specifically
- Current RTAT **below** baseline → Green (improved)
- Current RTAT **above** baseline → Red (worsened)
- +/- column follows the same logic: negative delta = green (days reduced), positive = red (days added)
- When a current value is **at or below 10D target** AND improved significantly → Bold green

---

## Slide Architecture (Pixel-Perfect)

### Slide Dimensions
- Standard widescreen: 13,716,000 × 7,543,800 EMU (13.333" × 7.5")

### Layout: Main Overview Slide

```
┌─────────────────────────────────────────────────────────┐
│ [Field Service] Title Line                              │ ← Title bar
├─────────────────────────────────────────────────────────┤
│                     Performance                          │ ← Section header (centered, bold)
├────────────────────────┬────────────────────────────────┤
│  URBAN — stats banner  │  RURAL — stats banner          │ ← Sub-headers (centered)
│  ┌──────────────────┐  │  ┌──────────────────────────┐  │
│  │ Perf Table       │  │  │ Perf Table               │  │ ← Tables: Servicer|Base|(4WK)|+/-
│  └──────────────────┘  │  └──────────────────────────┘  │
├────────────────────────┼────────────────────────────────┤
│    March Review        │      April Strategy            │ ← Section headers (centered, bold)
├────────────────────────┼────────────────────────────────┤
│ ☐  RTAT Review         │ ☐  RTAT Strategy              │
│ ▪  bullet points       │ ▪  bullet points              │
│ ┌──────────────────┐   │                                │
│ │ Handed Off Table │   │                                │
│ └──────────────────┘   │                                │
│ ☐  Pending Review      │ ☐  Pending Strategy           │
│ ▪  bullet points       │ ▪  bullet points              │
└────────────────────────┴────────────────────────────────┘
```

### Layout: Appendix Slide (ASM Breakdown)

```
┌─────────────────────────────────────────────────────────┐
│ [Field Service] RTAT — ASM Servicer Breakdown (Appendix)│
├────────────┬───────────┬────────────┬───────────────────┤
│ Graham     │ Graham    │ Brown      │ Brown             │
│ Urban      │ Rural     │ Urban      │ Rural             │
│ 10.0D(Mar) │ 12.6D(Mar)│ 9.3D(Mar)  │ 13.0D(Mar)       │
│ ┌────────┐ │ ┌───────┐ │ ┌────────┐ │ ┌───────────────┐ │
│ │Table   │ │ │Table  │ │ │Table   │ │ │Table          │ │
│ └────────┘ │ └───────┘ │ └────────┘ │ └───────────────┘ │
└────────────┴───────────┴────────────┴───────────────────┘
```

---

## Exact Formatting Specifications

### Font
- **Family:** Arial (always)
- **Title:** 15pt (190500 EMU), Bold, Black
- **Section Headers (Performance, March Review, April Strategy):** 12pt (152400), Bold, Black, Center-aligned
- **Sub-section Headers (☐ RTAT Review, ☐ Pending Strategy):** 10pt (127000), Bold, Black
- **Bullet Text:** 8pt (101600), Normal weight, Black (unless color-coded)
- **Table Header Row:** 7pt (88900), Bold, White on dark background
- **Table Data:** 7pt (88900), Normal weight, Black (unless color-coded)

### Shape Positioning (EMU coordinates)

| Element | Left | Top | Width | Height |
|---------|------|-----|-------|--------|
| Title | 274320 | 91440 | 9144000 | 320040 |
| "Performance" header | 274320 | 484632 | 11612880 | 228600 |
| Urban banner | 274320 | 749808 | 5669280 | 182880 |
| Rural banner | 6217920 | 749808 | 5669280 | 182880 |
| Urban perf table | 274320 | 960120 | 5669280 | 914400 |
| Rural perf table | 6217920 | 960120 | 5669280 | 914400 |
| "March Review" header | 274320 | 2450592 | 5623560 | 228600 |
| "April Strategy" header | 6217920 | 2450592 | 5669280 | 228600 |
| Left section headers (☐) | 457200 | varies | 5303520 | 210312 |
| Left bullets (▪) | 640080 | varies | 5120640 | 164592 |
| Right section headers (☐) | 6400800 | varies | 5303520 | 210312 |
| Right bullets (▪) | 6583680 | varies | 5120640 | 164592 |
| Vertical divider (left/right split) | 6035040 | varies | 0 | varies |

### Spacing
- Bullet line spacing: 182880 EMU (~0.2 inches)
- Section header to first bullet: 237744 EMU
- Between sections: ~200000 EMU gap

### Dividers / Lines
- Horizontal dividers: height=0, fill=#000000 (black hairline)
- Vertical divider between left/right: width=0, fill=#D0D0D0 (light gray)

### Tables

**Performance Tables (Urban/Rural top servicers):**
- Columns: Servicer | Base | (4WK) | +/-
- Header row: White text on dark background, bold
- Data rows: White fill
- (4WK) column: Green if improved, Red if worsened, Bold if ≤10D
- +/- column: Green if negative (improved), Red if positive (worsened)
- Prefix +/- values with + or - sign

**Handed Off Table:**
- Columns: Handed Off | Was | Now | +/-
- Same color rules as performance tables
- "Now" column: Bold green if ≤10D

**Appendix Tables (ASM breakdown):**
- Columns: Servicer | Base | (4WK)
- Same formatting, no +/- column

---

## Multi-Run Color Coding in Bullets

Some bullets have mixed colors within a single line. This requires multiple runs in the same paragraph:

**Example: "▪  Urban: 13.09D → 9.7D (Mar) — below 10D target"**
- Run 1: "▪  Urban: 13.09D → " → Black
- Run 2: "9.7D" → Bold Green (because improved)
- Run 3: " (Mar) — below 10D target" → Black

**Example: "▪  Rural: 11.33D → 12.8D (Mar) — Apr trending 11.4D"**
- Run 1: "▪  Rural: 11.33D → " → Black
- Run 2: "12.8D" → Red (because worsened)
- Run 3: " (Mar) — Apr trending " → Black
- Run 4: "11.4D" → Green (because trending down)

### When to Color-Code
- Metric values that represent performance → color by good/bad
- Labels, descriptions, framework text → always black
- Strategy bullets → generally all black (strategy is about approach, not specific metric values)

---

## Section Content Guidelines

### Review Sections (Left Column)

**RTAT Review:**
- Baseline → Current with delta
- Separate Urban and Rural lines
- Mention handed-off ASCs with before/after table
- Factual: what the numbers show

**Pending Review:**
- Where pending was when we started vs now
- Combined and per-ASM breakdown
- Total count trends, percentage trends
- NOT split by urban/rural (pending is holistic)

### Strategy Sections (Right Column)

**RTAT Strategy:**
- REPAIR framework (always include the letter bar)
- Which market is getting heavier focus and why
- Target progression (10D → 8D, tied to peak season not quarters)
- Describe the dynamic Top 10 methodology — not specific ASCs
- NO specific ASC names in strategy

**Pending Strategy:**
- Holistic approach (not urban/rural)
- Current % → target % with the goal stated
- What "done" looks like (only backorder parts left at 30+)
- How tracking works (daily dashboard, WoW measurement)
- Progression: 30+ → 25-30 → keep driving down

---

## How to Use This Template

### STEP ZERO — Every Time, No Exceptions

Before building or modifying ANY slide, do these two things:

1. **Read the reference screenshot:** `original slide screenshot.png` — visually confirm the layout, spacing, colors, and density. This is what the final product should look like. Claude can read images natively, so open this file first.
2. **Read this CLAUDE.md** — review the exact specs, color codes, and content rules.

This prevents format drift across conversations. The screenshot is the source of truth for "does it look right?" and this doc is the source of truth for "is it built right?"

### Building a New Month's Slides

1. Get the latest data from the Google Sheet (RTAT dashboard, pending tracker)
2. Update the performance tables with new Top 10 servicers
3. Update the banners (job counts, percentages, baseline → current)
4. Update Review sections with the month's actual results
5. Update Strategy sections (usually minor tweaks unless direction changes)
6. Update Appendix tables with per-ASM breakdown

### "Korean-ifying" Someone Else's Slides

When given slides in any format to convert:

1. **Identify what's Review vs Strategy** — separate them
2. **Strip opinions from Review** — just facts and numbers
3. **Strip specific names from Strategy** — describe the approach
4. **Apply color coding** — green for good, red for bad, everywhere
5. **Use the exact layout** — two-column bottom half, tables in top half
6. **Match fonts and sizes** — Arial, sizes per spec above
7. **Add dividers** — hairline black horizontals, gray vertical center split

### Data Sources

- **RTAT Data:** Google Sheet `11oT7rWM5LF8iz9iT2_kvlIDgn-oug5KxSqc1oVBO_K4`
- **Pending Data:** Google Sheet `18RHsOXUFUEFS6D1MgT2y3m0rvs8ihLMIZwxN1floGT4`
- **Dashboard KPIs:** `/home/daniel/projects/work/network-dashboard/data/dashboard_kpis.json`
- **Admin Config (goals):** `/home/daniel/projects/work/network-dashboard/data/admin_config.json`

### Key Metrics to Pull

| Metric | Source | Location |
|--------|--------|----------|
| Urban/Rural RTAT | RTAT Google Sheet | Per-ASM area tabs |
| Top 10 servicers | RTAT Google Sheet | Sorted by Impact Score |
| Pending 30+% | Dashboard KPIs JSON | `pending_30plus_pct` per ASM |
| Pending avg age | Dashboard KPIs JSON | `avg_age` per ASM |
| WoW deltas | Dashboard KPIs JSON | `wow_delta_*` fields |
| Goals | Admin config JSON | `goals.pending_30plus_pct`, `goals.top10_avg_age` |

---

## Files in This Project

| File | Purpose |
|------|---------|
| `MBR_VersionA_Template.pptx` | Current production slide deck |
| `MBR_VersionB_Story.pptx` | Alternate version (same content, different intent) |
| `FS MBR Apr 2026.pptx` | Original source deck from leadership |
| `Urban_RTAT_OnePager.pptx` | One-pager with Urban ASC details |
| `Rural_RTAT_OnePager.pptx` | One-pager with Rural ASC details |
| `Manager_Cheat_Sheet.docx` | Coverage guide for ASMs standing in for Daniel |
| `build_updates.py` | Script that modifies slide sections programmatically |
| `CONTEXT.md` | Data context — volume explanations, verified numbers |
| `original slide screenshot.png` | Reference screenshot of the target layout |

---

## Anti-Patterns (What NOT to Do)

1. **Don't put specific ASC names in Strategy sections** — "Engage Doctor Maint (37.0D)" belongs in talking points, not strategy slides
2. **Don't split pending by Urban/Rural** — pending is managed holistically
3. **Don't use "by Q3" or "by Q2"** — use "before peak season" or month references
4. **Don't use Western color schemes** — no blues, oranges, yellows for status. Green = good, Red = bad, Black = neutral. That's it.
5. **Don't add slide transitions, animations, or gradients** — clean, static, data-dense
6. **Don't use paragraph-based text boxes** — each bullet is its own shape (this is how python-pptx cloning works cleanly)
7. **Don't add logos or decorative elements** — the data IS the presentation
8. **Don't make slides "pretty" at the expense of density** — Korean leadership wants maximum information per slide, not white space
