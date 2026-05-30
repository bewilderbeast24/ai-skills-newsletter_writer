# Step: 01-plan-research

## Description
This stage involves defining the scope, mandatory topics, and research plan for the newsletter.

## Purpose
- Establish the project root directory. (Default Vs User input)
- Define the research scope (Exclusive vs. Additive).
- Map topics to research files.

## Pre-stage Checkpoint
### Version Control
- Check `git status` to ensure a clean state.If there's no git repo, initialize one with `git init`.
- Do not commit at this stage.

## Workflow

### Process
1. Create a root directory named after the topic in default root directory: `<newsletter-name>/`.
2. Analyze user input for `topic`(mandatory), `style-guide`(inferred, if not specified), and `topics_list` (inferred, if not specified) .
4. Create `<newsletter-name>/plan-research.md` detailing the plan for topics to be researched about.
5. Define scope:
   - `exclusive_scope: true`: Only cover user specified topics.
   - `exclusive_scope: false`: Agent adds relevant sub-topics (default mode).
6. List Research Topics and map them to `<newsletter-name>/Research/XX_[slug].md`. **DO NOT CREATE `<newsletter-name>/Research/` SUBDIRECTORY, YOU ARE ONLY REQUIRED TO MAP THE TOPICS TO A FILE IN RESEARCH SUBDIRECTORY FOR NEXT STEP.**

### Output Format
- Default Root Directory: `D:/personal-vault/20 Areas/Newsletters/`
- All documents stored within default directory in sub-directory named: `<newsletter-name>/`
- Final Research File: `<newsletter-name>/plan-research.md`

## Post-stage Checkpoint
### Progress Tracking
- Update `.agents/skills-diary/newsletter-writer/checklist.md` by marking "Phase 1: Research Planning" as completed.

### Version Control
- N/A.

### Human in the Loop (HITL)
- Present `plan-research.md` to the user for approval of the scope and topics.

### Auto pilot
- Proceed if all mandatory topics are included and the research plan is logically consistent.
