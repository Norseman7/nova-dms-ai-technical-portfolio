# File Relevance And Safety Review

## Manual Screenshot Publication Update

Screenshots were excluded during the automated preparation pass because visual evidence required manual review. After manual review, selected sanitized screenshots were added under:

- `portfolio/screenshots/dms/`
- `portfolio/screenshots/figma/`
- `portfolio/screenshots/nova/`

These screenshots are included as visual portfolio evidence only. They are not raw runtime evidence, full source publication, or complete system documentation. The screenshot filenames in the automated source review may differ from the final manually approved filenames.


All source candidates were evaluated from the local portfolio workspace using relative source paths. Local absolute paths are intentionally omitted from this GitHub-ready review file.

Optional subfolders under `docs/`, `nova/`, `dms/`, `figma_plugin/`, and `examples/` are used only to group evidence by reviewer question and evidence area.

| Source path | Proposed destination | Include / Exclude | Relevance score 0-5 | Safety status | Reason | Required cleanup |
| ----------- | -------------------- | ----------------: | ------------------: | ------------- | ------ | ---------------- |
| `.gitignore` | `-` | Exclude | 2 | EXCLUDE_NOT_RELEVANT | Safety patterns are useful locally but not needed as portfolio evidence. | None; exclude. |
| `AI_REVIEW_SUMMARY.md` | `docs/capability_and_role_alignment/AI_REVIEW_SUMMARY.md` | Include | 5 | SAFE | Concise AI/human screening summary. | None; copied as curated evidence. |
| `architecture/combined_system_view.md` | `docs/production_readiness/combined_system_view.md` | Include | 5 | SAFE | Combined NOVA/DMS/Figma system view. | None; copied as curated evidence. |
| `architecture/dms_governance_layer.md` | `dms/governance/dms_governance_layer.md` | Include | 5 | SAFE | DMS governance layer explanation. | None; copied as curated evidence. |
| `architecture/figma_design_workflow.md` | `figma_plugin/design_qc_workflow/figma_design_workflow.md` | Include | 5 | SAFE | Figma design-to-development workflow. | None; copied as curated evidence. |
| `architecture/human_in_the_loop_validation.md` | `docs/traceability_and_validation/human_in_the_loop_validation.md` | Include | 5 | SAFE | Human review and approval model. | None; copied as curated evidence. |
| `architecture/nova_data_pipeline.md` | `nova/architecture/nova_data_pipeline.md` | Include | 5 | SAFE | NOVA data pipeline and traceability flow. | None; copied as curated evidence. |
| `CAPABILITY_MATRIX.md` | `docs/capability_and_role_alignment/CAPABILITY_MATRIX.md` | Include | 5 | SAFE | Capability-to-evidence matrix for AI Solutions Engineer review. | None; copied as curated evidence. |
| `dms/ai_development_governance.md` | `dms/governance/ai_development_governance.md` | Include | 5 | SAFE | Governance for AI-assisted development. | None; copied as curated evidence. |
| `dms/architecture_protection_workflow.md` | `dms/architecture_protection/architecture_protection_workflow.md` | Include | 5 | SAFE | Architecture protection workflow. | None; copied as curated evidence. |
| `dms/audit_and_handover_workflow.md` | `dms/audit_and_handover/audit_and_handover_workflow.md` | Include | 5 | SAFE | Audit and handover continuity workflow. | None; copied as curated evidence. |
| `dms/dms_overview.md` | `dms/governance/dms_overview.md` | Include | 5 | SAFE | DMS governance system overview. | None; copied as curated evidence. |
| `dms/screenshots/DMS_screenshot_1.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `dms/screenshots/DMS_screenshot_2.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `dms/screenshots/DMS_screenshot_3.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `dms/screenshots/DMS_screenshot_4.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `dms/screenshots/DMS_screenshot_5.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `dms/screenshots/DMS_screenshot_6.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `dms/screenshots/DMS_screenshot_7.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `dms/screenshots/DMS_screenshot_8.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `dms/screenshots/DMS_screenshot_9.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `docs/industrial_relevance.md` | `docs/capability_and_role_alignment/industrial_relevance.md` | Include | 5 | SAFE | Industrial / E&P relevance summary. | None; copied as curated evidence. |
| `docs/industry_relevance_without_company_names.md` | `-` | Exclude | 1 | EXCLUDE_NOT_RELEVANT | File does not directly support the curated repository purpose or is not mapped to an evidence area. | None; exclude. |
| `docs/PAM_AI_Technical_Portfolio_NOVA_DMS_FINAL.pdf` | `portfolio/PAM_AI_Technical_Portfolio_NOVA_DMS_FINAL.pdf` | Include | 5 | SAFE_AFTER_CLEANUP | Final portfolio PDF; primary reviewer artifact. | No content cleanup required; scan hit is benign exclusion/safety wording. |
| `docs/paul_role_and_contribution.md` | `docs/capability_and_role_alignment/paul_role_and_contribution.md` | Include | 5 | SAFE | Role positioning and contribution evidence. | None; copied as curated evidence. |
| `docs/production_readiness_mindset.md` | `docs/production_readiness/production_readiness_mindset.md` | Include | 5 | SAFE | Production-readiness mindset and safeguards. | None; copied as curated evidence. |
| `docs/technical_complexity_summary.md` | `docs/production_readiness/technical_complexity_summary.md` | Include | 5 | SAFE | Compact technical complexity summary. | None; copied as curated evidence. |
| `docs/transferable_ai_engineering_capability.md` | `docs/capability_and_role_alignment/transferable_ai_engineering_capability.md` | Include | 5 | SAFE | Transferable AI engineering capability framing. | None; copied as curated evidence. |
| `docx_output/PAM_AI_Technical_Portfolio_NOVA_DMS_DRAFT_04.docx` | `-` | Exclude | 0 | EXCLUDE_OUTDATED | Draft or intermediate portfolio artifact; final PDF is preferred. | None; exclude. |
| `docx_output/PAM_AI_Technical_Portfolio_NOVA_DMS_DRAFT_05.docx` | `-` | Exclude | 0 | EXCLUDE_OUTDATED | Draft or intermediate portfolio artifact; final PDF is preferred. | None; exclude. |
| `docx_output/PAM_AI_Technical_Portfolio_NOVA_DMS_FINAL.docx` | `-` | Exclude | 2 | EXCLUDE_UNVERIFIED | Editable Word artifact is not needed for GitHub evidence package; final PDF is preferred. | None; exclude. |
| `docx_output/portfolio_docx_draft_04_report.md` | `-` | Exclude | 0 | EXCLUDE_OUTDATED | Draft or intermediate portfolio artifact; final PDF is preferred. | None; exclude. |
| `docx_output/portfolio_docx_draft_05_report.md` | `-` | Exclude | 0 | EXCLUDE_OUTDATED | Draft or intermediate portfolio artifact; final PDF is preferred. | None; exclude. |
| `docx_output/~$M_AI_Technical_Portfolio_NOVA_DMS_DRAFT_04.docx` | `-` | Exclude | 0 | EXCLUDE_NOISY | Word lock/temporary file. | None; exclude. |
| `docx_output/~$M_AI_Technical_Portfolio_NOVA_DMS_DRAFT_05.docx` | `-` | Exclude | 0 | EXCLUDE_NOISY | Word lock/temporary file. | None; exclude. |
| `examples/ai_reasoning_boundary_example.md` | `examples/validation_traceability/ai_reasoning_boundary_example.md` | Include | 5 | SAFE | AI reasoning boundary example. | None; copied as curated evidence. |
| `examples/architecture_protection_example.md` | `examples/architecture_protection/architecture_protection_example.md` | Include | 5 | SAFE | Sanitized architecture protection example. | None; copied as curated evidence. |
| `examples/audit_workflow_example.md` | `examples/audit_workflow/audit_workflow_example.md` | Include | 5 | SAFE | Sanitized audit workflow example. | None; copied as curated evidence. |
| `examples/data_quality_and_session_boundary_example.md` | `examples/architecture_protection/data_quality_and_session_boundary_example.md` | Include | 4 | SAFE | Data quality and session-boundary example. | None; copied as curated evidence. |
| `examples/design_qc_workflow_example.md` | `examples/design_qc_workflow/design_qc_workflow_example.md` | Include | 5 | SAFE | Sanitized design QC workflow example. | None; copied as curated evidence. |
| `examples/event_detection_pseudocode.md` | `examples/event_detection_pseudocode/event_detection_pseudocode.md` | Include | 5 | SAFE | Sanitized event detection pseudocode. | None; copied as curated evidence. |
| `examples/validation_traceability_example.md` | `examples/validation_traceability/validation_traceability_example.md` | Include | 5 | SAFE | Sanitized traceability example. | None; copied as curated evidence. |
| `figma_plugin/design_to_development_bridge.md` | `figma_plugin/design_qc_workflow/design_to_development_bridge.md` | Include | 5 | SAFE | Figma-to-Codex design handoff bridge. | None; copied as curated evidence. |
| `figma_plugin/figma_plugin_overview.md` | `figma_plugin/design_qc_workflow/figma_plugin_overview.md` | Include | 5 | SAFE | Figma plugin supporting workflow overview. | None; copied as curated evidence. |
| `figma_plugin/screenshots/FIGMA_Screenshot_1.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `figma_plugin/ui_quality_control_workflow.md` | `figma_plugin/design_qc_workflow/ui_quality_control_workflow.md` | Include | 5 | SAFE | UI quality-control workflow. | None; copied as curated evidence. |
| `LIMITATIONS_AND_MATURITY.md` | `docs/maturity_and_limitations/LIMITATIONS_AND_MATURITY.md` | Include | 5 | SAFE_AFTER_CLEANUP | Honest maturity limits and non-claims. | No content cleanup required; scan hit is benign exclusion/safety wording. |
| `nova/analysis_and_brain_architecture.md` | `nova/brain_store/analysis_and_brain_architecture.md` | Include | 5 | SAFE | Analysis and Brain architecture boundary. | None; copied as curated evidence. |
| `nova/brain_store_and_learning_model.md` | `nova/brain_store/brain_store_and_learning_model.md` | Include | 5 | SAFE | Brain Store and learning model boundary. | None; copied as curated evidence. |
| `nova/event_architecture_scope.md` | `nova/event_model/event_architecture_scope.md` | Include | 5 | SAFE | Event architecture scope and boundaries. | None; copied as curated evidence. |
| `nova/event_detection_and_validation.md` | `nova/event_model/event_detection_and_validation.md` | Include | 5 | SAFE | Event detection and validation methodology. | None; copied as curated evidence. |
| `nova/high_volume_data_challenge.md` | `nova/architecture/high_volume_data_challenge.md` | Include | 5 | SAFE | High-volume market data complexity and design response. | None; copied as curated evidence. |
| `nova/module_registry_and_contracts.md` | `nova/event_model/module_registry_and_contracts.md` | Include | 5 | SAFE | Module registry and contract discipline. | None; copied as curated evidence. |
| `nova/nova_architecture.md` | `nova/architecture/nova_architecture.md` | Include | 5 | SAFE | NOVA layered architecture evidence. | None; copied as curated evidence. |
| `nova/nova_overview.md` | `nova/architecture/nova_overview.md` | Include | 5 | SAFE | NOVA purpose, domain, modules, and maturity. | None; copied as curated evidence. |
| `nova/nova_roadmap.md` | `nova/roadmap/nova_roadmap.md` | Include | 4 | SAFE | Roadmap and maturity framing. | None; copied as curated evidence. |
| `nova/screenshots/NOVA_Screenshot_1.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `nova/screenshots/NOVA_Screenshot_2.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `nova/screenshots/NOVA_Screenshot_3.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `nova/screenshots/NOVA_Screenshot_4.png` | `-` | Exclude | 0 | EXCLUDE_UNVERIFIED | Screenshot/image evidence is not manually approved for publication in this task. | Do not include; manual visual approval required. |
| `nova/standardized_outcome_model.md` | `nova/event_model/standardized_outcome_model.md` | Include | 5 | SAFE | Outcome model and validation boundary. | None; copied as curated evidence. |
| `portfolio_master.md` | `-` | Exclude | 0 | EXCLUDE_OUTDATED | Draft or intermediate portfolio artifact; final PDF is preferred. | None; exclude. |
| `portfolio_master_draft_02.md` | `-` | Exclude | 0 | EXCLUDE_OUTDATED | Draft or intermediate portfolio artifact; final PDF is preferred. | None; exclude. |
| `portfolio_master_draft_03.md` | `-` | Exclude | 0 | EXCLUDE_OUTDATED | Draft or intermediate portfolio artifact; final PDF is preferred. | None; exclude. |
| `portfolio_master_draft_05.md` | `-` | Exclude | 0 | EXCLUDE_OUTDATED | Draft or intermediate portfolio artifact; final PDF is preferred. | None; exclude. |
| `PORTFOLIO_PREP_REPORT.md` | `-` | Exclude | 2 | EXCLUDE_NOISY | Preparation/build report is useful internally but too noisy for public evidence repository. | None; exclude. |
| `PROJECT_EVIDENCE_INDEX.md` | `-` | Exclude | 3 | EXCLUDE_DUPLICATE | Source index is replaced by a GitHub-ready evidence index of included files. | None; exclude. |
| `README.md` | `-` | Exclude | 3 | EXCLUDE_DUPLICATE | Source README is replaced by GitHub-ready README tailored to this repository. | None; exclude. |
| `SPEC_REVIEW_EVIDENCE_EXTRACTION_REPORT.md` | `-` | Exclude | 2 | EXCLUDE_NOISY | Preparation/build report is useful internally but too noisy for public evidence repository. | None; exclude. |
| `SYSTEM_COMPLEXITY_MAP.md` | `docs/production_readiness/SYSTEM_COMPLEXITY_MAP.md` | Include | 5 | SAFE | Complexity driver, risk, and design-response map. | None; copied as curated evidence. |
| `TECHNICAL_ARCHITECTURE_DEEP_DIVE.md` | `docs/production_readiness/TECHNICAL_ARCHITECTURE_DEEP_DIVE.md` | Include | 5 | SAFE | System-of-systems architecture and control/data/validation flows. | None; copied as curated evidence. |
| `tools/render_portfolio_master.py` | `-` | Exclude | 0 | EXCLUDE_OUTDATED | Draft or intermediate portfolio artifact; final PDF is preferred. | None; exclude. |
| `tools/render_portfolio_master_draft_02.py` | `-` | Exclude | 0 | EXCLUDE_OUTDATED | Draft or intermediate portfolio artifact; final PDF is preferred. | None; exclude. |
| `tools/render_portfolio_master_draft_03.py` | `-` | Exclude | 0 | EXCLUDE_OUTDATED | Draft or intermediate portfolio artifact; final PDF is preferred. | None; exclude. |
| `TRACEABILITY_AND_VALIDATION_MODEL.md` | `docs/traceability_and_validation/TRACEABILITY_AND_VALIDATION_MODEL.md` | Include | 5 | SAFE | Traceability and validation model from output back to evidence. | None; copied as curated evidence. |
