# Figma Design Workflow

## Workflow Model

```text
Figma selected scope
-> structured export
-> review / naming cleanup
-> preview validation
-> scoped apply
-> verified design state
-> Codex implementation prompt
-> human review
```

## Role In Portfolio

The Figma workflow is a supporting design-to-development control layer. It helps make UI work inspectable, scoped, and reviewable.

## Controls

| Control | Purpose |
| --- | --- |
| Selected-scope authority | Prevents uncontrolled global edits. |
| Structured export | Makes design hierarchy and properties reviewable. |
| Preview validation | Shows differences before mutation. |
| Scope matching | Blocks stale or mismatched change sets. |
| Naming consistency | Improves implementation readability. |
| Human apply | Keeps final mutation under human control. |

## Codex Bridge

Once a Figma scope is reviewed, Paul can use the structured output to guide Codex implementation with clearer names, layout intent, and acceptance criteria.
