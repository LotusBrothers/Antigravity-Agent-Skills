---
name: brainstorming
description: Explores user intent, requirements, and design before implementation. Use this skill before any creative work, creating features, or modifying behavior to turn ideas into fully formed designs and specs through natural collaborative dialogue.
---

# Brainstorming Ideas Into Designs

## When to use this skill
- Before creating new features, building components, or adding functionality.
- When starting an ambiguously defined task or ticket.
- Whenever a user asks to "brainstorm", "design", or "plan" a new idea conceptually.

## Workflow

You MUST complete these items in order:

1. [ ] **Explore project context:** Check files, docs, and recent commits.
2. [ ] **Ask clarifying questions:** Ask questions one at a time to understand purpose, constraints, and success criteria. Prefer multiple-choice questions.
3. [ ] **Propose 2-3 approaches:** Present options with trade-offs and recommend one.
4. [ ] **Present design sections:** Scale each section to its complexity. Get user approval after each section (Architecture, components, data flow, error handling, testing).
5. [ ] **Write design doc:** Save the validated design to `docs/plans/YYYY-MM-DD-<topic>-design.md` and commit it.
6. [ ] **Transition to implementation:** Invoke the `planning` skill to create a detailed implementation plan.

## Instructions

- **One question at a time:** Do not overwhelm the user with multiple questions.
- **YAGNI ruthlessly:** Remove unnecessary features from all designs.
- **Incremental validation:** Present the design and get approval before moving on.
- **Gate:** Do NOT invoke any implementation skill, write code, or scaffold a project until the design is approved and you transition to the `planning` skill.

## Resources
- Ensure you have read access to the current project context for exploration.
