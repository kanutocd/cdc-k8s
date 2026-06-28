# KEDA.md

## Purpose
- Describe how KEDA enables event-driven scaling for CDC workers.

## Scaling Approach
- Workers are scaled based on external metrics (e.g., event backlog, oldest event age).
- CDC reader remains a singleton; only workers scale up/down.

## Metric Conventions
- Standardize Prometheus metrics (e.g., `mammoth_event_backlog`, `mammoth_oldest_event_age_seconds`).
- Define thresholds and standard queries for scaling.

## ScaledObject Templates
- Provide a standard `ScaledObject` YAML snippet.
- Fields: `scaleTargetRef` (worker deployment), `triggers`, `thresholds`, polling intervals, and cooldown periods.

## Best Practices
- Always scale workers—not the replication reader.
- Ensure scale-to-zero policies are defined when idle.
- Document scaling profiles for backlog, event age, or other CDC-relevant metrics.