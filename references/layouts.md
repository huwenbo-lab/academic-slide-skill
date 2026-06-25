# Locked Academic Layouts

Use these layouts as the canonical vocabulary for this skill. A deck may omit layouts, but it should not invent decorative structures when one of these roles fits. For HTML decks, each `<section class="slide">` should use a `data-layout` value from this list.

## A01_TITLE — Title and affiliation

Use for the opening slide. It contains context metadata, title, subtitle/topic line, presenter name, department, university, date, and an optional crest. The title should be the research title or a talk-specific claim, not a vague theme.

## A02_SECTION — Section divider

Use sparingly to mark major transitions: theory, design, results, interpretation, conclusion, backup. The page is mostly empty and uses a large teal section title. Do not add bullets.

## A03_RESEARCH_PUZZLE — Empirical or theoretical puzzle

Use near the beginning. The slide should articulate a tension: what existing theory would lead us to expect, what empirical reality complicates it, and why the discrepancy matters. Use one strong headline and at most three short supporting lines.

## A04_LITERATURE_GAP — What prior work leaves unresolved

Use to organize literature without a dense citation dump. Structure around two or three literatures or claims, then identify the unresolved question. Citations can appear in a small note line, but the slide should be conceptual rather than bibliographic.

## A05_THEORY_FRAMEWORK — Theoretical mechanism or conceptual model

Use to show causal logic, normative structure, or mechanism. Keep nodes few and meaningful. Avoid complex arrow diagrams unless the argument genuinely requires them. The framework should make later hypotheses or empirical tests intelligible.

## A06_EXPECTATIONS — Hypotheses, expectations, or competing predictions

Use when the talk requires explicit propositions. Each expectation should be short and testable. If there are competing mechanisms, show them as parallel pathways or a compact comparison table.

## A07_DATA_DESIGN — Data, sample, and research design

Use for survey, administrative, panel, experiment, factorial vignette, conjoint, or qualitative comparative designs. The audience should be able to see who is observed, what varies, what is measured, and what comparison identifies the claim.

## A08_MEASUREMENT — Key variables and operationalization

Use when concepts require careful measurement. Show construct, operational indicator, scale/coding, and interpretive caveat. Do not list every control variable; controls belong in notes or backup.

## A09_METHOD_MODEL — Estimation or identification logic

Use for model family, fixed effects, causal identification, weighting, clustering, imputation, or design-based inference. The slide should explain why the model matches the question, not merely display an equation.

## A10_MAIN_RESULT_FIGURE — Primary finding

Use for the central empirical result. One claim, one figure, one model note. The headline should state the substantive result. The figure should be large enough to read from the back of a room.

## A11_INTERACTION_OR_HETEROGENEITY — Conditional patterns

Use for subgroup differences, interactions, marginal effects, predicted probabilities, or stratified models. Do not show interaction coefficients alone. Show the pattern as predicted values, slopes, contrasts, or marginal effects.

## A12_MECHANISM_RESULT — Evidence about mechanism

Use when results adjudicate between mechanisms or explain why the main result occurs. Pair the result with a short interpretation: what mechanism is supported, weakened, or left unresolved.

## A13_TABLE_SUMMARY — Compact empirical table

Use only when a table is superior to a figure. Limit rows and columns to the argument. Use explicit labels rather than variable-name abbreviations. Put full regression tables in backup.

## A14_ROBUSTNESS — Robustness and sensitivity summary

Use to show which alternative specifications or checks change the result. Organize as “Stable,” “Partially sensitive,” and “Remaining concern,” or as a compact row-by-check matrix. Do not make the slide a list of everything tried.

## A15_LIMITATIONS_SCOPE — Scope conditions and limitations

Use to define what the evidence does and does not establish. A strong limitation slide improves credibility when it is precise. Avoid vague apology language.

## A16_CONTRIBUTIONS — Contributions and takeaway

Use near the end. Separate theoretical, empirical, and methodological contributions when relevant. Contributions should be stated as changes to how the audience should think about the topic.

## A17_DISCUSSION_QA — Questions or seminar discussion

Use for discussion prompts, workshop feedback requests, or Q&A. Questions should be substantive and connected to the paper’s next revision, not generic “any questions?” placeholders.

## A18_CLOSING — Final slide

Use for thank-you, contact, and final claim. In a research talk, the closing should restate the paper’s core contribution in one sentence.

## A19_BACKUP_APPENDIX — Backup slide

Use for extended tables, alternative codings, additional samples, full models, survey items, or extra figures. Backup slides may be denser but must remain readable.

## Layout selection rules

Every slide needs one dominant function. If a slide tries to combine theory, data, model, and result, split it. If a result slide needs extensive method explanation to be understood, add an earlier method/design slide. If a literature slide contains more than six citations, convert it into a conceptual gap slide and move the bibliography to backup.
