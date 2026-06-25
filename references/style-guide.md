# Academic Swiss Style Guide

## Design position

The visual style should communicate institutional affiliation and scholarly restraint. It is not an official university brand manual. It is a practical academic presentation system derived from an HKU-style slide template: small course/context label at the top-left, compact crest position at the top-right, large teal headings, charcoal text, and low-decorative content layouts.

## Palette

| Token | Hex | Use |
|---|---:|---|
| `--academic-teal` | `#006D6B` | Primary institutional accent, slide titles, section markers, thin rules, selected chart series |
| `--ink` | `#1A1A1A` | Main text, figure labels, axes, high-emphasis annotation |
| `--muted` | `#555555` | Notes, captions, secondary metadata, model notes |
| `--rule` | `#E7E6E6` | Hairlines, separators, subtle table rules, light panels |
| `--paper` | `#FFFFFF` | Main background |
| `--off-paper` | `#F7F8F7` | Optional section-break or backup-slide background |

Optional chart accents should remain subordinate to the main teal:

| Accent | Approx. hex | Use |
|---|---:|---|
| Turquoise | `#02B28C` | Secondary series in two-group comparisons |
| Sky blue | `#019CD5` | Third series or confidence-band accent |
| Red-orange | `#F04023` | Negative case, exception, contrast, not a default highlight |
| Gold | `#FCCC28` | Rare emphasis; avoid large fills |
| Dark brown | `#613621` | Not recommended except in logo-derived artwork |

## Typography

Use a clean sans-serif system. For English: Aptos, Calibri, Helvetica Neue, Arial, Source Sans, or IBM Plex Sans. For Chinese: Noto Sans CJK, Source Han Sans, PingFang SC, Microsoft YaHei, or system sans. Do not use decorative script, playful display fonts, overly condensed techno fonts, or generic startup-deck typography.

Recommended PPT scale at 16:9:

| Element | Size range | Weight | Notes |
|---|---:|---:|---|
| Title slide title | 44–56 pt | 600–700 | Use teal, max two lines |
| Section title | 40–50 pt | 600–700 | Sparse page, strong pause |
| Content slide headline | 30–38 pt | 600–700 | Write as claim, not label |
| Body text | 20–26 pt | 400–500 | Keep paragraphs short |
| Figure labels | 16–20 pt | 400–500 | Never below legible size |
| Footnotes/model notes | 11–14 pt | 400 | Only essential metadata |

For HTML at 1920×1080, use equivalent pixel sizes: slide title 64–82px, content headline 44–56px, body 28–36px, notes 18–22px.

## Layout and grid

Use a stable page frame. Top-left contains course, talk, or context metadata. Top-right may contain a crest or affiliation mark. The main title block starts left-aligned, usually around 8–10% from the left edge. Use a single vertical axis across slides whenever possible.

Avoid card-heavy dashboard styling. A slide can use one large figure, a two-column comparison, or a single framework diagram, but it should not look like an interactive UI. Academic slides should have a page-like structure rather than app-like modular panels.

## Logo and crest use

A crest or institutional logo is an affiliation marker. It should be small, consistently placed, and not repeated inside the body area. Use it on the title slide, section slides, and closing slide by default. For formal institutional teaching decks, a small top-right crest on every slide is acceptable. For external conferences, use it only on the title and closing slides unless the user asks otherwise.

Never use a crest as a watermark, background texture, icon, sticker, or decorative motif. Never recolor, distort, crop, or apply shadows to a crest.

## Chart style

Use figures as evidence devices. Prefer direct labels over crowded legends. Highlight the focal group or focal coefficient in teal and de-emphasize reference or comparison groups in gray. Use red-orange only for anomalies, rejected hypotheses, or negative contrasts. Always include uncertainty where it matters: confidence intervals, standard errors, credible intervals, or transparent model notes.

## Tables

Tables should be analytic summaries, not software output. Use few columns, generous row spacing, and minimal rules. Full regression tables belong in backup unless the table itself is the object of explanation.

## Tone

The visual tone is restrained, exacting, and credible. It should look appropriate in a sociology/demography workshop, dissertation committee meeting, or professional conference room. The ideal audience reaction is not “beautiful deck,” but “the argument and evidence are unusually clear.”
