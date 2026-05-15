# Act Explainer Newsletter Style Guide

This style guide focuses on conceptual, first-principles explanations of specific Acts and Regulations. It breaks down complex legislation into logical, manageable "sub-areas" and uses visual aids to map out the legal landscape.

## Tone & Voice
- **Tone**: Analytical, pedagogical, and investigative.
- **Voice**: Explanatory and logic-driven. Avoid "because the law says so" in favor of "here is why this logic was necessary."
- **First Principles**: Always start with the core problem. Introduce the complication that makes a simple solution impossible, then show how the legal provision solves it.
- **De-mystification**: Treat legal artifacts (Acts, Sections, Rules) not as authorities to be obeyed, but as the final "endpoint" of a specific train of thought.

## Writing Steps (The Logical Build-Up)
Every topic within the newsletter should follow this logical progression:
1. **Phase 1: The Raw Need**: Why do we need a rule here at all? What is the fundamental conflict?
2. **Phase 2: The Complications**: What "edge cases" or conflicting interests make a simple rule fail?
3. **Phase 3: The Legal Synthesis**: How does the specific Section or Regulation reconcile these complications?
4. **The Artifact as Endpoint**: Only introduce specific legal citations (e.g., "Section 158BA") after the logic for its existence has been established.

---

## Mandatory Episode Structure

### Episode 1: Introduction to <act-name>
This episode sets the stage for the entire series.
1. **The Purpose**: Give a brief introduction on what's the point of the requested Act. Why does it exist? What system does it regulate?
2. **The Structural Map**: Give an outline of all chapters and what subpoints of the main point are dealt with in each of these chapters. 
    - **Requirement**: Use a **Markdown Table** or **Mermaid Diagram** for this outline.

### Subsequent Episodes: <chapter-name-in-act>
Every subsequent episode must focus on a specific chapter of the Act.
1. **Context**: Reiterate the subpoint dealt with in the current chapter (linked back to the structural map in Episode 1).
2. **The Breakdown**: Break the given chapter into distinct **sub-areas** which all sections in the given chapter cover.
    - **Requirement**: Use a **Markdown Table** to list these sub-areas and their general purpose.
3. **Sub-Area Deep Dives**: For each sub-area identified above, create a sub-header and include:
    - **3.1 Visual Flow**: A **Mermaid chart** to show the topics dealt with in the sub-area and their logical connections.
    - **3.2 Exhaustive Section-by-Section**: Create a sub-sub-header for each sub-area and list **ALL** sections belonging to that sub-area. For every section, provide a concise but complete explanation of its purpose. **No sections from the chapter should be omitted.**

---

## Formatting Standards
- **Completeness Mandate**: Every single section number in the chapter must appear exactly once across the sub-areas of the episode.
- **Logical Callouts**: Use `> **The Logic**: ...` to highlight the core reasoning behind a provision.

- **Visuals-First**: Every sub-area MUST have a Mermaid chart.
- **Navigational Clarity**: Ensure each chapter episode references its place in the overall Act structure.

## Prohibitions
- **No Rote Recitation**: Never just list sections or clauses without explaining their underlying "why."
- **No Jargon-First Explanations**: Never lead with a technical legal term; lead with the concept it represents.
- **No Skipping Chapters**: If the Act is being covered, every relevant chapter should ideally get its own episode or clear placement.
