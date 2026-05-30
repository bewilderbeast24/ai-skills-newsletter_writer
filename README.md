# Newsletter Writer Skill

A specialized Gemini CLI skill for automating the creation of high-quality, research-driven, multi-episode newsletter series.

## Overview

The `newsletter-writer` skill follows a structured 4-phase sequential workflow to transform a simple topic into a comprehensive series of newsletter episodes. It emphasizes deep research, logical planning, and adherence to specific style guides to ensure professional and engaging content.

## Key Features

- **Structured Workflow**: Sequential phases for planning, research, and writing.
- **Deep Research**: Automated gathering of findings for multiple sub-topics.
- **Multi-Episode Planning**: Intelligent mapping of research to a logical episode structure.
- **Style Guide Adherence**: Generates content aligned with specific brand voices or writing styles.
- **Progress Tracking**: Built-in checklist for monitoring development across all phases.
- **HITL & Autopilot Modes**: Supports both "Human-in-the-Loop" for granular control and "Autopilot" for faster generation.

## Workflow Phases

1.  **Research Planning**: Define the scope, mandatory topics, and map out the research files.
2.  **Research Execution**: Gather detailed findings and data for each planned sub-topic.
3.  **Newsletter Planning**: Map research to episodes, plan visuals, and create the introductory episode.
4.  **Newsletter Writing**: Draft episodes sequentially and generate a final episode index.

## Directory Structure

Generated newsletters are organized within a dedicated project folder:

```text
<newsletter-name>/
├── Episodes/
│   ├── 00-introduction-to-newsletter.md
│   ├── 01-episode-one.md
│   └── ...
├── Research/
│   ├── 01-research-topic.md
│   └── ...
├── plan-research.md
└── plan-newsletter.md
```

## How to Use

To use this skill, ensure it is available in your Gemini CLI environment. You can trigger it by asking Gemini to "Write a newsletter about [Topic]" or "Start a new newsletter project".

### Input Requirements
- **Newsletter Topic**: The core subject of your series.
- **Style Guide** (Optional): A specific style or voice to follow (defaults to inferred if not provided).
- **Topics List** (Optional): Specific sub-topics you want to ensure are covered.

## Installation

This skill is designed to be used with the [Gemini CLI](https://github.com/google/gemini-cli). Copy this directory into your `.gemini/skills/` folder or include it in your project's skill path.

---
*Created as part of the AI Skills ecosystem.*
