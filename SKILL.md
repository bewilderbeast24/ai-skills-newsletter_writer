---
name: newsletter-writer
description: Creates a detailed multi-episode newsletter in markdown with research, planning, and writing phases, all organized within a single project directory.
---

# Newsletter Writer

## Skill Overview
The `newsletter-writer` skill automates the creation of comprehensive, multi-episode newsletter series. It follows a structured 4-phase sequential workflow to ensure deep research, logical planning, and high-quality writing aligned with specific style guides. All project files are contained within a dedicated root folder.

## Workflow Sequence

| Stage | Description | Workflow | Input | Output |
| :--- | :--- | :--- | :--- | :--- |
| **1. Research Planning** | Define scope, mandatory topics, and map research files. | [01-plan-research.md](assets/01-plan-research.md) | `newsletter-topic`(mandatory), `style-guide` (inferred if not given), `topics_list` (inferred if not given) | [plan-research.md](references/output-formats/plan-research.md) |
| **2. Research Execution** | Gather findings and data for each sub-topic. | [02-execute-research.md](assets/02-execute-research.md) | Generated `<newsletter-name>/plan-research.md` | No fixed format |
| **3. Newsletter Planning** | Map research to episodes, plan visuals, and create introductory episode. | [03-plan-newsletter.md](assets/03-plan-newsletter.md) | Researched files in `<newsletter-name>/Research/` | [plan-newsletter.md](references/output-formats/plan-newsletter.md) and [intro](references/output-formats/introduction-to-newsletter.md) |
| **4. Newsletter Writing** | Draft episodes sequentially and generate final episode index. | [04-write-newsletter.md](assets/04-write-newsletter.md) | Generated `<newsletter-name>/plan-newsletter.md` | No fixed format |

## Pre-stage Checkpoint
- **Human in the Loop (HITL)**: Default. Confirm the research plan (Phase 1), researched topics (Phase 2), episode layout (Phase 3) and newsletter drafting (Phase 4) before closing the respective phase.
- **Autopilot**: If requested, the agent will autonomously handle topic expansion and writing based on the initial topic.

## Core Operation Flow

### Progress Tracking
Before starting, ensure a checklist in the format of [checklist.md](references/checklist.md) is initialized in `.agents/skills-diary/newsletter-writer/<newsletter-name>/checklist.md`.

After completing each phase below, you MUST update relevant checklist by marking the corresponding checkbox as completed (`[x]`).

### Execution
Follow the steps in `assets/` sequentially:
1. **[01-plan-research.md](assets/01-plan-research.md)**: Create `<newsletter-name>/plan-research.md`.
2. **[02-execute-research.md](assets/02-execute-research.md)**: Using the `plan-research.md` from Stage 1, populate `<newsletter-name>/Research/`.
3. **[03-plan-newsletter.md](assets/03-plan-newsletter.md)**: Using the researched files from Stage 2, create `<newsletter-name>/plan-newsletter.md` and `<newsletter-name>/Episodes/00-introduction-to-newsletter.md`.
4. **[04-write-newsletter.md](assets/04-write-newsletter.md)**: Using the `plan-newsletter.md` from Stage 3, populate `<newsletter-name>/Episodes/` and append index to `00-introduction-to-newsletter.md`.

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
    plan-research.md
    plan-newsletter.md
```
- All episodes are verified against the plan and style guide.
- The project directory is presented to the user.
- Feedback is solicited for future improvements.

## Additional Instructions
All temporary scripts generated while execution of skills (scripts which will be deleted after execution) will be written in `.agents/skills-diary/temp-scripts/<timestamp>/` as directory
