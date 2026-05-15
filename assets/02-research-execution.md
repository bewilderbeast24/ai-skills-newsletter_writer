# Step: 02-research-execution

## Description
This stage involves gathering detailed information for each planned topic.

## Purpose
- Build a knowledge base for the newsletter.
- Capture key findings, data tables, and diagrams.
- Ensure all mandatory topics are thoroughly researched.

## Pre-stage Checkpoint
### Version Control
- Ensure `<newsletter-name>/` exists.

## Workflow

### Output Format
- Default Root Directory: `D:/personal-vault/20 Areas/Writing/Newsletters/`
- All documents stored within default directory in sub-directory named: `<newsletter-name>/Research/`
- Files: `<newsletter-name>/Research/*.md`

### Process
1. Create the `<newsletter-name>/Research/` directory.
2. For each topic in `<newsletter-name>/plan_research.md`, create a file `<newsletter-name>/Research/XX_[slug].md`.
3. Conduct research and populate files with:
   - Key Findings.
   - Important Details (using **Tables**).
   - Relationships/Flows (using **Mermaid**).
   - Source citations.

## Post-stage Checkpoint
### Version Control
- Verify files are created: `dir <newsletter-name>/Research/`.

### Human in the Loop (HITL)
- Briefly summarize the findings of the research phase to the user.

### Auto pilot
- Proceed if all topics in `plan_research.md` have corresponding research files.
