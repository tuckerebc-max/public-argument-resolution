# Public Argument Resolution package contract

**Registry ID:** `SKILL-PAR`  
**Package version:** `0.1.0`  
**Source domain:** `DOM-PAR`  
**Current status:** `READY_WITH_CONDITIONS` and explicit-review only

## Required inputs

Supply a bounded public issue, question at issue, affected public, purpose, authority, jurisdiction or institution, mode, constraints, access and rights conditions, criteria or decision rule, available sources, and review route. Missing authority or criteria stops the run.

## Core payload

The package produces `public_issue_contract`, `stasis_map`, `stakeholder_map`, `competing_position_map`, `evidence_provenance_ledger`, `comparison_record`, `process_plan`, `decision_rule`, `dissent_uncertainty_record`, `ai_transformation_log`, `decision_or_unresolved_record`, and `human_review_route` inside the shared artifact envelope.

## Quality conditions

The package preserves disagreement, affected-party visibility, source conflict, rights, access, authority, criteria, feasibility, legitimacy, dissent, uncertainty, human confirmation, and reviewability. It distinguishes recommendation, decision, settlement, adjudication, and unresolved record.

## Canonical source paths

See `catalog/source-manifest.json` for the portable mapping to the prompt, corpus crosswalk, competency design specification, technical specification, and textbook architecture. The source validation IDs are `TST-PAR-001` through `TST-PAR-012`, plus `TST-INT-007` and `TST-INT-008`.
