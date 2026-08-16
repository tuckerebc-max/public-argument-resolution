# Public Argument Resolution

Standalone GitHub repository for the Main textbook skill `SKILL-PAR` and competency `COMP-PAR-RESOLUTION`.

Upload this folder as the repository root. It includes `SKILL.md`, Codex UI metadata, competency and assessment codification, evaluator specification, output schema, handoff contract, public-review and decision-gate guidance, provenance and authorship guidance, source manifest, shared schemas, fixtures, validation scripts, CI, release metadata, and checksums.

## Canonical design trace

`SPEC-PAR-001` · `ANRI-DOM-PAR-001` · `ARCH-PAR-001` · `CORP-PAR-001`

This package remains explicitly conditional and is finalized as a private draft. It requires a responsible human authority and review route. It does not make autonomous legal, civic, health, policy, disciplinary, or other high-stakes decisions. `SPEC-PAR-001` has no synthetic `FR-PAR-*` list; its evaluator preserves the controlled-entity, workflow, and human-review design.

## Validate locally

```text
python scripts/validate_repository.py
python scripts/validate_repository.py --check
python scripts/evaluate_package.py
python scripts/build_release_manifest.py --check
```

The canonical textbook source files remain external and are mapped, not copied, in `catalog/source-manifest.json`.
