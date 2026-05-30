# Step: 01-research-planning

## Description
This stage involves defining the scope, mandatory topics, and research plan for the newsletter.

## Purpose
- Establish the project root directory.
- Define the research scope (Exclusive vs. Additive).
- Map topics to research files.

## Pre-stage Checkpoint
### Version Control
- Check `git status` to ensure a clean state.
- Do not commit at this stage.

## Workflow

### Output Format
- Default Root Directory: `D:/personal-vault/20 Areas/Writing/Newsletters/`
- All documents stored within default directory in sub-directory named: `<newsletter-name>/`
- Final Research File: `<newsletter-name>/plan_research.md`

### Process
1. Create a root directory named after the topic in default root directory: `<newsletter-name>/`.
2. Analyze user input for `topic`(mandatory), `style_guide`(inferred, if not specified), and `topics_list` (inferred, if not specified) .
4. Create `<newsletter-name>/plan_research.md` detailing the plan for topics to be researched about.
5. Define scope:
   - `exclusive_scope: true`: Only cover user specified topics.
   - `exclusive_scope: false`: Agent adds relevant sub-topics (default mode).
6. List Research Topics and map them to `<newsletter-name>/Research/XX_[slug].md`. **DO NOT CREATE `<newsletter-name>/Research/` SUBDIRECTORY, YOU ARE ONLY REQUIRED TO MAP THE TOPICS TO A FILE IN RESEARCH SUBDIRECTORY FOR NEXT STEP.**

## Post-stage Checkpoint
### Version Control
- N/A.

### Human in the Loop (HITL)
- Present `plan_research.md` to the user for approval of the scope and topics.

### Auto pilot
- Proceed if all mandatory topics are included and the research plan is logically consistent.
