# DMS Governance Layer

## Purpose

DMS provides the governance and continuity layer for controlled AI-assisted software development. It supports NOVA and other development projects by keeping project context, documentation, audit activity, task records, and review gates structured and traceable.

## Governance Model

```text
Project context
  -> document categories
  -> handovers
  -> audit templates
  -> task/time records
  -> reports
  -> review gates
  -> next-session continuity
```

## Governance Controls

| Control | Purpose |
| --- | --- |
| Project selection | Keeps document and report context aligned to the active project. |
| Document categories | Separates handovers, specs, as-built records, authority, governance, validation, and debug material. |
| Audit templates | Define bounded inspection workflows with clear scope and non-scope. |
| Handover protocol | Prevents context loss between sessions. |
| Task tracking | Ties work to concrete objectives and timing. |
| Agent/governance files | Keep ChatGPT and Codex behavior aligned with project rules. |
| Reports | Provide deterministic review outputs. |

## Architecture Protection Role

DMS supports NOVA by making architecture protection repeatable. It keeps data authority, UI/backend boundaries, module isolation, protected areas, and documentation authority visible during review.
