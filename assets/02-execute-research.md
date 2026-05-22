# Step: 02-execute-research

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

### Process
1. Using the `plan-research.md` from Stage 1, proceed to create the `<newsletter-name>/Research/` directory.
2. For each topic in `<newsletter-name>/plan-research.md`, create a file `<newsletter-name>/Research/XX_[slug].md`.
3. Conduct research and populate files with:
   - Key Findings.
   - Important Details (using **Tables**).
   - Relationships/Flows (using **Mermaid**).
   - Source citations.

### Output Format
- Default Root Directory: `D:/personal-vault/20 Areas/Writing/Newsletters/`
- All documents stored within default directory in sub-directory named: `<newsletter-name>/Research/`
- Files: `<newsletter-name>/Research/*.md`

## Post-stage Checkpoint
### Progress Tracking
- Update `.agents/skills-diary/newsletter-writer/checklist.md` by marking "Phase 2: Research Execution" as completed.

### Version Control
- Verify files are created: `dir <newsletter-name>/Research/`.

### Human in the Loop (HITL)
- Briefly summarize the findings of the research phase to the user.

### Auto pilot
- Proceed if all topics in `plan_research.md` have corresponding research files.
