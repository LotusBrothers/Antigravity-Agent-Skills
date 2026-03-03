---
name: planning
description: Writes comprehensive, step-by-step implementation plans for a multi-step task before touching code. Use this skill when you have a spec or requirements and need to detail how the engineering work should be executed task-by-task.
---

# Writing Implementation Plans

## When to use this skill
- After brainstorming and obtaining an approved design document.
- When the user provides a clear spec or requirements for a multi-step task.
- Before writing any code for a complex feature.

## Workflow

1. [ ] **Create Plan Document:** Initialize a new file at `docs/plans/YYYY-MM-DD-<feature-name>.md`.
2. [ ] **Write Header:** Include the Goal, Architecture, and Tech Stack.
3. [ ] **Define Tasks:** Break the work into 2-5 minute bite-sized tasks.
4. [ ] **Detail Each Task:** Include exact file paths, specific code snippets (DRY, YAGNI, TDD), and exact commands for testing and committing.
5. [ ] **Offer Execution Options:** Ask the user how they want to proceed (e.g., executing tasks one by one).

## Instructions

- Write the plan assuming the executor has zero context for the codebase.
- Document exactly which files to create/modify, what tests to write, and how to verify.

### Task Structure Template
Use the following format for each bite-sized task in the plan:

```markdown
### Task N: [Component Name]

**Files:**
- Create: `exact/path/to/file.ext`
- Modify: `exact/path/to/existing.ext:123-145`

**Step 1: Write failing test**
(Insert specific code snippet)

**Step 2: Run test to verify it fails**
Run: `[test command]`
Expected: FAIL

**Step 3: Write minimal implementation**
(Insert specific code snippet)

**Step 4: Run test to verify it passes**
Run: `[test command]`
Expected: PASS

**Step 5: Commit**
`git add [files]`
`git commit -m "feat: [description]"`
```

## Resources
- Refer to `docs/plans/` for existing examples if needed.
