# Halcyon Assessment Operations

Operations repository for the Q4 2026 certification assessment cycle.

## Layout

- `registry/assessment_registry.csv` - authoritative exam registry.
- `intake/cycle_brief.json` - intake ticket for the active cycle.
- `out/exam_manifest.jsonl` - published per-candidate manifest read by the scheduling system.
- `docs/manifest_schema.md` - record schema for the manifest.

## Registry conventions

The registry is grouped. Each exam event starts with a row that records the programme code,
cohort label, delivery mode, exam date and time slot. The rows immediately below it are
continuation rows: they leave those columns blank and record the room, seats, candidate ID
range and lead invigilator for one allocation of that event.

`cohort_label` is the exam event's own label. It identifies exactly the cohort or cohorts that
sit the recorded event.
