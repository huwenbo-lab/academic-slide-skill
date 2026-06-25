---
name: academic-slide-skill
description: Create restrained, argument-driven academic presentations for social science, sociology, demography, population studies, family, marriage, stratification, dissertation, workshop, seminar, conference, and job-talk contexts. Use when the user needs scholarly PPT/HTML slides with HKU-informed academic styling, claim-based headlines, figure-first results, and controlled low-decoration layouts.
---

# Academic Slide Skill

This skill creates academic slide decks whose visual and rhetorical goal is **scholarly clarity**. It is calibrated for social-science PhD and research work, especially sociology, demography, population studies, family, marriage, social stratification, survey research, factorial vignette experiments, conjoint experiments, and quantitative empirical conference or workshop talks.

The default visual system is **HKU Academic Swiss**: white or near-white canvas, a restrained deep-teal accent, charcoal body text, generous margins, a small crest slot only when institutionally appropriate, and layouts that foreground research argument, empirical design, figures, and interpretation.

## What this skill is for

Use this skill when the user asks for an academic presentation, conference talk, workshop deck, dissertation defense deck, job-talk draft, research progress presentation, literature-review presentation, seminar slides, teaching discussion deck, or an existing PPT/PPTX to be redesigned in a more scholarly style.

Do not use this style for product launches, marketing decks, startup pitch decks, motivational keynotes, decorative magazine decks, or general-purpose commercial slideware unless the user explicitly asks for an academic treatment.

## Core design thesis

The deck should look like a well-structured empirical article translated into a live talk. Each slide must perform one identifiable argumentative action: pose a puzzle, locate a literature gap, define a concept, show a design, report a finding, interpret a mechanism, address robustness, state a limitation, synthesize contributions, or invite focused discussion.

Visual design is subordinate to inference and credibility. Use design to make hierarchy, comparison, and evidence legible. Do not use design to compensate for unclear claims.

## Default output format

If the user needs editable slides for a conference, class, workshop, committee meeting, or dissertation defense, create `.pptx` unless they requested HTML. If the user wants a browser-based deck, create a single HTML presentation or an HTML deck with a local `assets/` folder. When making HTML, use `assets/template-hku-academic.html` as the starting point and validate with `scripts/validate-academic-slide-deck.mjs`.

## Minimal clarification before drafting

If the user already supplied slides, a paper, abstract, tables, figures, or a detailed brief, begin work without asking a long question list. Ask only questions that materially affect the deck. If information is missing and cannot be inferred, ask at most three questions:

1. What is the talk situation: conference, workshop, dissertation defense, teaching, job talk, or internal meeting?
2. How long is the talk, and should the deck be speaker-led or reading-first?
3. Should institutional branding be visible, minimal, or absent?

If the user provides only a topic, create a provisional talk spine and mark assumptions explicitly in a working note before generating the deck.

## Workflow

### 1. Build the argument spine before slide design

Create a compact outline using this sequence unless the user supplied a stronger structure:

`Research puzzle → Literature gap → Theoretical claim → Data/design → Measurement → Model/identification → Main finding → Mechanism/heterogeneity → Robustness/scope → Contributions → Discussion/Q&A`

For a 12–15 minute conference talk, compress this into 10–14 content slides plus title and closing. For a 30–45 minute workshop, expand the methods, mechanisms, and robustness sections. For a job talk or defense, create a main deck plus backup slides.

### 2. Choose a density mode

Use **speaker-led mode** for live talks: short headlines, fewer words, large figures, limited bullet text, and a strong oral narrative. Use **reading-first mode** for circulated seminar materials: more self-contained slides, slightly denser annotations, and more explicit sample/model notes. Never make slides so dense that a table, footnote, model note, or axis label becomes unreadable.

### 3. Use locked academic layouts

Use only the layouts defined in `references/layouts.md`. Each slide should declare one layout role in speaker notes, slide metadata, or HTML `data-layout`. Do not improvise decorative layouts when an academic layout exists. If a new layout is genuinely needed, document why it is not covered by the existing taxonomy.

The most common layouts are title, section break, research puzzle, literature gap, theoretical framework, data/design matrix, measurement, method/model, main result figure, mechanism/heterogeneity figure, model/table summary, robustness summary, limitation/scope condition, contribution, discussion, and backup.

### 4. Apply the Academic Swiss style

Use the style guide in `references/style-guide.md`. The default institutional accent is deep teal `#006D6B`; primary text is charcoal `#1A1A1A`; secondary text is `#555555`; background is white or off-white. Use other accent colors only for charts or categorical distinctions.

Keep the crest or logo small. Use it as institutional identification, not ornament. In normal academic talks, a crest belongs on the title slide, section breaks, and closing slide; content slides may use a small top-right crest only if the user prefers consistent institutional branding.

### 5. Write slide headlines as claims

Avoid descriptive headings such as “Regression Results,” “Background,” or “Literature Review.” Prefer analytic headlines such as “Higher female earnings reduce expected domestic responsibility more than male earnings increase it.” A title should tell the audience what to learn from the slide before they inspect the figure or table.

### 6. Present results figure-first

Do not paste raw software output. Transform coefficients, interactions, predicted probabilities, marginal effects, or subgroup contrasts into a figure whenever possible. Each result slide should contain one main result, one figure or compact table, one interpretive headline, and a small model/sample note.

For regression tables, show only coefficients needed for the claim. Put full models in backup. For interaction terms, show predicted values or marginal effects; do not make the audience infer the substantive pattern from a coefficient alone.

### 7. Preserve academic credibility

Every empirical claim needs enough methodological context to be assessable: sample, outcome, key predictors, model family, controls, and uncertainty indication. Use short notes instead of dense paragraphs. A slide may be visually polished and still fail if it hides how the finding was produced.

### 8. Validate and revise

Before delivery, run the checklist in `references/checklist.md`. For HTML decks, run:

```bash
node scripts/validate-academic-slide-deck.mjs path/to/deck.html
```

Revise until there are no P0 errors. For PPTX decks, manually inspect title hierarchy, alignment, logo use, figure readability, and table density in slide-show mode.

## Hard constraints

Never use neon gradients, random icon grids, excessive shadows, decorative 3D objects, emoji, stock-photo filler, or product-launch visual tropes. Never shrink empirical tables below readable size. Never bury the main finding in a paragraph. Never use an institutional crest as a wallpaper, watermark, repeating pattern, or decorative badge unless the user explicitly requests an institutional poster rather than an academic talk.
