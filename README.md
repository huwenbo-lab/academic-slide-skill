# Academic Slide Skill

A standalone academic presentation skill for creating restrained, argument-driven slide decks for sociology, demography, family, stratification, population studies, and other social-science research talks.

This repository is designed for coding agents such as Claude Code, Codex, Cursor, or other local agents with filesystem access. The skill helps turn abstracts, paper drafts, regression tables, figures, old PPT files, or rough notes into scholarly presentations with clear argument structure and controlled visual style.

## Design position

The default visual system is **HKU Academic Swiss**: white or near-white canvas, deep teal accent, charcoal text, small institutional crest slot, large claim-based titles, restrained rules, and figure-first result pages. It is calibrated from a user-provided HKU presentation template that used course/context metadata, title and subtitle hierarchy, section dividers, two-column comparison slides, discussion questions, and a closing slide.

The goal is not to make slides look like a product launch, consulting deck, or generic AI-generated template. The goal is scholarly clarity: the audience should understand the research question, theory, design, result, mechanism, limitation, and contribution quickly enough to follow the live argument.

## What it creates

The skill can generate or improve:

- Conference talks
- Workshop or seminar decks
- Dissertation defense slides
- Job-talk research presentations
- Research progress presentations
- Literature-review presentations
- Academic teaching or reading-discussion decks
- HTML browser-based decks when editable `.pptx` output is not required

## Repository structure

```text
academic-slide-skill/
├── SKILL.md
├── README.md
├── LICENSE
├── package.json
├── assets/
│   └── template-hku-academic.html
├── references/
│   ├── academic-talk-structures.md
│   ├── checklist.md
│   ├── layouts.md
│   ├── result-figure-rules.md
│   └── style-guide.md
├── scripts/
│   └── validate-academic-slide-deck.mjs
└── examples/
    └── sample-talk-outline.md
```

## Basic use

In a coding-agent environment, point the agent at this repository and ask it to use `SKILL.md`.

Example:

```text
Use the academic-slide-skill from this repository to turn my paper abstract, figures, and regression tables into a 15-minute sociology conference presentation.
```

For HTML decks, start from `assets/template-hku-academic.html` and run:

```bash
npm run validate -- path/to/deck.html
```

For editable PowerPoint decks, apply the same style guide and locked layout taxonomy while generating `.pptx` files.

## Logo and institutional-note policy

This repository does not commit an HKU crest image. It defines a crest slot and an HKU-informed color/style system, but public or external use should follow institutional logo-use rules. If the deck is not an official HKU teaching or institutional presentation, keep branding minimal: use affiliation on the title and closing slides, not as repeated decoration.

## License

The code and written skill materials in this repository are released under the MIT License, unless otherwise noted. University names, marks, and logos are not licensed by this repository.
