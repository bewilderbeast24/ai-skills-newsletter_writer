# Step: 04-write-newsletter

## Description
This stage involves drafting the actual newsletter episodes following the selected style guide.

## Purpose
- Produce high-quality, formatted markdown episodes.
- Maintain consistent tone and flow across the series.
- Incorporate planned visuals and navigation.

## Pre-stage Checkpoint
### Version Control
- NA

## Workflow

### Process
1. Using the `plan-newsletter.md` from Stage 3, proceed to create the `<newsletter-name>/Episodes/` directory (if not already created).
2. Select and read the appropriate style guide from `references/style_guides/<applicable-style-guide>.md`.
3. Write episodes sequentially (`01-<slug>.md`, `02-<slug>.md`, etc.) based on the plan.
4. For each episode, ensure it conforms to following default values, if no overriding values are provided by user:
   - Length: 300-500 words.
   - Visuals: Include planned Tables/Mermaid.
   - Structure: Overview, Content, Key Takeaways, Navigation links.
5. Cross-reference previous episodes to ensure continuity.
6. Once all episodes are drafted, return to `00-introduction-to-newsletter.md` and append an 'Episode Index' section. This section must contain a list of links to every created episode, using the episode's title as the display text (e.g., `[Introduction to AI](01-intro-to-ai.md)`).

### Output Format
- Default Root Directory: `D:/personal-vault/20 Areas/Writing/Newsletters/`
- All documents stored within default directory in sub-directory named: `<newsletter-name>/Episodes/`
- Final Newsletter Plan File: `<newsletter-name>/Episodes/*.md`

## Post-stage Checkpoint
### Progress Tracking
- Update `.agents/skills-diary/newsletter-writer/checklist.md` by marking "Phase 4: Newsletter Writing" as completed.

### Version Control
- Verify files: `dir <newsletter-name>/Episodes/`.
- Verify `00-introduction-to-newsletter.md` if all newsletters are indexed and linked before handover.

### Human in the Loop (HITL)
- Present the final episodes to the user for review and approval.

### Auto pilot
- Finalize if all planned episodes are written and formatted correctly.
