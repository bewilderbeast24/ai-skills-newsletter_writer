# Step: 04-newsletter-writing

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

### Output Format
- Default Root Directory: `D:/personal-vault/20 Areas/Writing/Newsletters/`
- All documents stored within default directory in sub-directory named: `<newsletter-name>/Episodes/`
- Final Newsletter Plan File: `<newsletter-name>/Episodes/*.md`

### Process
1. Create the `<newsletter-name>/Episodes/` directory.
2. Select and read the appropriate style guide from `references/style_guides/<applicable-style-guide>.md`.
3. Write episodes sequentially (`01-<slug>.md`, `02-<slug>.md`, etc.).
4. For each episode, ensure it conforms to following default values, if no overriding values are provided by user:
   - Length: 300-500 words.
   - Visuals: Include planned Tables/Mermaid.
   - Structure: Overview, Content, Key Takeaways, Navigation links.
5. Cross-reference previous episodes to ensure continuity.

## Post-stage Checkpoint
### Version Control
- Verify files: `dir <newsletter-name>/Episodes/`.

### Human in the Loop (HITL)
- Present the final episodes to the user for review and approval.

### Auto pilot
- Finalize if all planned episodes are written and formatted correctly.
