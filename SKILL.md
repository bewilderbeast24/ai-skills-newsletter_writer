---
name: newsletter-writer
description: Creates a detailed multi-episode newsletter in markdown with research, planning, and writing phases, all organized within a single project directory.
---

# Newsletter Writer

## Skill Overview
The `newsletter-writer` skill automates the creation of comprehensive, multi-episode newsletter series. It follows a structured 4-phase sequential workflow to ensure deep research, logical planning, and high-quality writing aligned with specific style guides. All project files are contained within a dedicated root folder.

## Workflow Sequence

| Stage | Description | Workflow |
| :--- | :--- | :--- |
| **1. Research Planning** | Define scope, mandatory topics, and map research files. | [01-research-planning.md](assets/01-research-planning.md) |
| **2. Research Execution** | Gather findings and data for each sub-topic. | [02-research-execution.md](assets/02-research-execution.md) |
| **3. Newsletter Planning** | Map research to episodes, plan visuals, and create introductory episode. | [03-newsletter-planning.md](assets/03-newsletter-planning.md) |
| **4. Newsletter Writing** | Draft episodes sequentially and generate final episode index. | [04-newsletter-writing.md](assets/04-newsletter-writing.md) |

## Pre-stage Checkpoint
- **Human in the Loop (HITL)**: Default. Confirm the research plan (Phase 1) and episode layout (Phase 3) before proceeding.
- **Autopilot**: If requested, the agent will autonomously handle topic expansion and writing based on the initial topic.

## Core Operation Flow

### Setup
Invoke with topic and optional parameters:
```text
/newsletter topic: [topic], style_guide: [DEFAULT_STYLE | RICHARD_FEYNMAN | PYTHON_EXPERT | ACT_EXPLAINER | AUDIT_EXPLAINER], topics_list: [list]
```

### Execution
Follow the steps in `assets/` sequentially:
1. **[01-research-planning.md](assets/01-research-planning.md)**: Create `<newsletter-name>/plan_research.md`.
2. **[02-research-execution.md](assets/02-research-execution.md)**: Populate `<newsletter-name>/Research/`.
3. **[03-newsletter-planning.md](assets/03-newsletter-planning.md)**: Create `<newsletter-name>/plan_newsletter.md` and `<newsletter-name>/Episodes/00-introduction-to-newsletter.md`.
4. **[04-newsletter-writing.md](assets/04-newsletter-writing.md)**: Populate `<newsletter-name>/Episodes/` and append index to `00-introduction-to-newsletter.md`.

## Handover & Confirmation
- The following directory is made ready (assuming newsletter is generated in default directory `D:/personal-vault/20 Areas/Newsletters/`):
```text
<newsletter-name>
    Episodes/
        00-introduction-to-newsletter.md
        <episode-01>
        <episode-02>
        ...
    Research/
        01-<research-aspect-01>.md
        02-<research-aspect-02>.md
        ...
    plan_research.md
    plan_newsletter.md
```
- All episodes are verified against the plan and style guide.
- The project directory is presented to the user.
- Feedback is solicited for future improvements.

## Additional Instructions
All temporary scripts generated while execution of skills (scripts which will be deleted after execution) will be written in `.gemini/skills-diary/temp-scripts/<timestamp>/` as directory
