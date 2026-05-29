# Design QC Workflow Example

## Scenario

A Figma design section contains generic layer names that make implementation ambiguous.

## Controlled Workflow

```text
1. Select the exact Figma subtree.
2. Export the selected scope.
3. Identify generic names and supported property changes.
4. Preview proposed rename/settings changes.
5. Confirm no unsupported structural changes are included.
6. Apply validated changes inside the selected scope.
7. Re-export the scope after apply.
8. Use the cleaned structure in the Codex implementation task.
```

## Safeguards

- The selected scope limits change impact.
- Preview makes changes reviewable before mutation.
- Unsupported edits block before apply.
- Human acceptance remains required.
