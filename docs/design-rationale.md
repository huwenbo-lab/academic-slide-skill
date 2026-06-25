# Design Rationale

## Why this is a standalone repository

This repository is intended to be a personal academic slide skill rather than a subdirectory inside a broader skill-architecture reading repository. The target use case is practical deck production: turning paper drafts, abstracts, empirical figures, tables, old PPT files, and talk notes into scholarly slides.

## Relationship to existing slide skills

The repository borrows a general engineering pattern common to coding-agent skills: a root `SKILL.md`, reusable `assets/`, reference files under `references/`, examples, and validation scripts. It does not vendor or copy an external slide generator’s source code. The academic presentation logic, style guide, layout taxonomy, result-figure rules, and validator are written as a separate system for social-science research presentations.

## Why the default style is restrained

Social-science academic talks have different constraints from product decks or public-facing keynotes. The slides need to make theoretical claims, research designs, empirical comparisons, uncertainty, and scope conditions legible. Excessive animation, decorative icons, gradient backgrounds, and product-style cards can make a deck look polished while weakening its scholarly credibility.

## Why the template uses HKU-informed cues but not an HKU logo asset

The user-provided reference presentation uses HKU-style conventions: course/context metadata, institutional affiliation, section dividers, two-column content, discussion questions, and closing slides. This repository translates those cues into a reusable academic style system: deep teal titles, charcoal text, a small crest slot, and clean content pages.

The actual institutional crest is not committed. Public repositories should avoid distributing university marks unless logo-use rules are clear. When making a private deck, a local crest image can be placed in `local-assets/` or inserted during deck generation.

## Preferred deck philosophy

A good academic slide deck should behave like an argument, not a document dump. Every slide should answer one question: Why does this puzzle matter? What does the literature miss? What is the mechanism? What is the comparison? What does the result show? What alternative explanations remain? What does the paper contribute?
