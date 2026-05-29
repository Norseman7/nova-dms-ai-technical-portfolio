# File Relevance And Safety Review

## Public Repository Boundary

This repository is a curated, sanitized evidence package prepared to support review of an AI technical portfolio. It is company-neutral and does not include the application-specific technical portfolio PDF.

The public repository is intended to show selected evidence of:

- controlled AI-assisted development
- NOVA architecture and evidence modeling
- DMS governance and continuity workflow
- validation, traceability, and human-in-the-loop safeguards
- selected Figma/design quality-control workflow
- selected sanitized examples and screenshots

It is not the real NOVA repository, the real DMS repository, a runtime repository, a full source-code publication, or an autonomous decision system.

## Manual Screenshot Publication Update

Screenshots were excluded during the automated preparation pass because visual evidence required manual review. After manual review, selected sanitized screenshots were added under:

- `portfolio/screenshots/dms/`
- `portfolio/screenshots/figma/`
- `portfolio/screenshots/nova/`

These screenshots are included as visual portfolio evidence only. They are not raw runtime evidence, full source publication, or complete system documentation. The screenshot filenames in the automated source review may differ from the final manually approved filenames.

## Inclusion Rules

Every included file should satisfy both conditions:

1. It directly supports the portfolio purpose.
2. It is publication-safe for a public repository.

## Included Evidence Areas

| Evidence area | Included location | Relevance | Safety status |
| --- | --- | --- | --- |
| Repository orientation | `README.md`, `PORTFOLIO_ACCESS_NOTE.md`, `PROJECT_EVIDENCE_INDEX.md` | Helps reviewers understand the repository purpose and navigation. | Safe public text. |
| Capability and role alignment | `docs/capability_and_role_alignment/` | Maps project evidence to AI solution design, technical judgement, and human ownership. | Sanitized Markdown only. |
| Production-readiness and complexity | `docs/production_readiness/` | Shows architecture, system complexity, safeguards, and maturity framing. | Sanitized Markdown only. |
| Traceability and validation | `docs/traceability_and_validation/`, `examples/validation_traceability/` | Shows evidence lineage, validation boundaries, and human-in-the-loop review. | Sanitized Markdown only. |
| NOVA architecture | `nova/architecture/` | Documents source authority, high-volume data handling, and data/evidence model boundaries. | Sanitized Markdown only. |
| NOVA event model | `nova/event_model/` | Documents event detection, outcome separation, module contracts, and validation framing. | Sanitized Markdown only. |
| Brain Store boundary | `nova/brain_store/` | Documents planned AI reasoning and evidence accumulation boundaries. | Sanitized Markdown only. |
| DMS governance | `dms/` | Shows audit, handover, architecture protection, and AI-assisted development governance. | Sanitized Markdown only. |
| Figma/design workflow | `figma_plugin/` | Shows design quality-control and Figma-to-development workflow discipline. | Sanitized Markdown only. |
| Sanitized examples | `examples/` | Provides compact examples without exposing real source code or raw data. | Sanitized Markdown only. |
| Supporting screenshots | `portfolio/screenshots/` | Provides selected visual evidence of DMS, NOVA, and Figma/design workflow surfaces. | Manually reviewed screenshots only. |

## Excluded Material

| Material | Reason for exclusion |
| --- | --- |
| Application-specific technical portfolio PDF | Submitted separately when relevant; excluded from this public repo to keep the repository company-neutral. |
| Real NOVA source repository | Not part of the public evidence package. |
| Real DMS source repository | Not part of the public evidence package. |
| Raw data / datasets / training sessions | Protected/noisy runtime material, not needed for public evidence. |
| Credentials, environment files, tokens, local caches | Sensitive or irrelevant to public portfolio review. |
| Runtime logs and temporary diagnostics | Noisy and potentially sensitive. |
| Draft DOCX/PDF/Markdown outputs | Superseded by final public evidence structure or submitted separately. |
| Full source-code publication | The purpose is portfolio evidence, not public release of implementation code. |
| Unapproved screenshots | Visual evidence requires manual review before publication. |

## Known Documentation Boundary

The application-specific PDF was intentionally removed from the public repository. Any references to a separately submitted technical portfolio should be read as referring to application/interview material outside this public repository.

## Final Safety Position

The public evidence package is intended to be readable without running NOVA or DMS. It should support review of architecture, governance, traceability, validation discipline, and controlled AI-assisted development while avoiding sensitive implementation material, raw data, credentials, or unsupported maturity claims.
