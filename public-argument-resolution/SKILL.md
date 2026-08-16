---
name: public-argument-resolution
description: Structure public disagreement and bounded deliberation through issue framing, stasis, affected parties, competing arguments, evidence and provenance, decision criteria, authority, feasibility, legitimacy, dissent, uncertainty, review routes, and human confirmation. Use for classroom deliberation, policy recommendation planning, public argument comparison, mediation or ADR preparation, and auditable decision records. Do not make autonomous high-stakes legal, civic, health, policy, or disciplinary decisions.
---

# Public Argument Resolution

## Invocation and status

Use explicitly while this package remains conditional. Keep a responsible human authority and review route visible at every consequential step.

## Workflow

1. Contract the public issue. Record issue, question at issue, affected public, purpose, authority, jurisdiction or institution, mode, constraints, rights/access conditions, and review or appeal route. If these are missing, return `NEEDS_ISSUE`, `NEEDS_AUTHORITY`, `NEEDS_MODE`, `NEEDS_CRITERIA`, or `NEEDS_REVIEW_ROUTE`.
2. Build the stasis map. Record fact, definition, interpretation, cause/consequence, value, policy, and meta-stasis or authority disagreements. Preserve multiple nodes when the controversy is not one question.
3. Represent affected parties and positions. Record stakeholders, interests, rights, access needs, power conditions, strongest recognizable claims, reasons, evidence, warrants, qualifiers, objections, consequences, and uncertainty. Do not infer a group's view without evidence.
4. Audit evidence and provenance. Require source IDs, locators, authority, method or basis, currency, relevance, limitations, corroboration, direct-reading status, rights status, and transformation log.
5. Compare under declared criteria. Make relevance, evidentiary sufficiency, inferential strength, rights compatibility, feasibility, distributional effects, reversibility, and responsiveness to alternatives visible. Do not collapse them into an unexplained score.
6. Declare the decision rule. Identify who or what has authority, threshold or procedure, criteria weights if any, non-negotiable constraints, and what the rule cannot decide.
7. Protect dissent and uncertainty. Record serious objections, minority positions, contested evidence, missing information, implementation risks, and conditions for revision.
8. Create the appropriate record: recommendation, decision, settlement, adjudication, unresolved record, or request for more evidence. Record the responsible human authority, date/version, alternatives considered, dissent, review route, and next action.
9. Run human-review QA. Confirm provenance, currentness, rights, accessibility, consent where relevant, AI-use disclosure, learner or participant decisions, and high-stakes boundaries before release.

## Mode rules

- Classroom deliberation requires fair participation, listening, evidence comparison, uncertainty, and learner decisions; it is not winner-take-all adjudication.
- Debate requires declared format, burden, evidence, response, and adjudication rules; a judge's decision is not proof of truth.
- Policy recommendation requires responsible authority, options, impacts, constraints, implementation, and review conditions.
- Legal or policy analysis requires jurisdiction, applicable authority, interpretive method, and currentness; this package is not legal advice.
- Mediation or ADR requires consent, roles, interests, terms, enforceability, and review; do not force consensus.

## Guardrails

- Never invent current law, policy, public facts, stakeholder positions, decision authority, consent, or evidence.
- Return `HIGH_STAKES_REFUSAL` for autonomous high-stakes decisions.
- Return `MISSING_WARRANT`, `WEAK_ALTERNATIVE`, `SOURCE_CONFLICT`, `RIGHTS_REVIEW`, or `CURRENTNESS_REVIEW` rather than smoothing away the problem.
- Do not ghostwrite a learner's final public position; preserve the learner or participant's substantive decision.

## Output contract

Return the shared artifact envelope with a PAR payload containing `public_issue_contract`, `stasis_map`, `stakeholder_map`, `competing_position_map`, `evidence_provenance_ledger`, `comparison_record`, `process_plan`, `decision_rule`, `dissent_uncertainty_record`, `ai_transformation_log`, `decision_or_unresolved_record`, and `human_review_route`.

## Handoffs

- Accept Argumentation records only when claim, evidence, strongest alternative, uncertainty, affected parties, authority, and decision-rule inputs are visible.
- Send missing evidence or unresolved causal reasoning back to QUEST or Argumentation.
- Route every consequential decision record to `HUMAN_REVIEW` with provenance, dissent, authority, learner decisions, and AI-use log preserved.

Read [skill-contract.md](references/skill-contract.md), [public-review-and-decision-gates.md](references/public-review-and-decision-gates.md), [handoff-contracts.md](references/handoff-contracts.md), [provenance-rights-authorship.md](references/provenance-rights-authorship.md), [output-schema.json](references/output-schema.json), and [evaluation-fixtures.json](references/evaluation-fixtures.json) as needed.
