# AI Development Governance

## Governance Principle

ChatGPT and Codex are used as development accelerators, not as uncontrolled owners of the system. Paul retains responsibility for domain logic, architecture direction, review, testing expectations, acceptance, and operational meaning.

## Controlled Workflow

| Control | Purpose |
| --- | --- |
| Task headers and scope | Keep each work session tied to a concrete objective. |
| Scope and non-scope | Prevent adjacent refactors or uncontrolled expansion. |
| Root cause before fix | Reduce assumption-based changes. |
| Implementation gates | Require entry point, state model, guardrails, and success criteria before material work. |
| Patch discipline | Favor bounded changes when a system is already working. |
| Human checks | Require human validation for UI, interaction, visual behavior, or user-facing logic. |
| Handover protocol | Preserve context between sessions and require review before continuation. |
| Approval states | Make acceptance, fixes, or rejection explicit. |

## AI Boundary

AI may help:

- draft specifications
- inspect code and documentation
- propose implementation plans
- produce review summaries
- generate controlled documentation
- identify risks and missing tests

AI must not:

- silently redefine architecture
- bypass human validation
- treat generated output as accepted truth
- modify protected source/data areas without scope
- promote unvalidated conclusions into trusted evidence

## Portfolio Relevance

This governance model demonstrates practical AI-assisted engineering control: prompt discipline, traceability, review gates, and clear separation between AI support and human accountability.
