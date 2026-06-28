# HELM.md

## Purpose
- Define Helm chart conventions for CDC ecosystem components.

## Chart Structure
- Standard Helm chart structure: `Chart.yaml`, `values.yaml`, `templates/`.
- CDC-specific values guidance (e.g., replicas for reader vs. worker).

## Versioning
- Align chart versions with application versions.
- SemVer conventions.

## Packaging & Releasing
- Use `helm package` for chart packaging.
- Release via Helm repo (e.g., GitHub Pages).

## Dependencies
- Document external chart dependencies (if applicable).
- Ensure dependency versions are pinned and audited.

## Best Practices
- Document common `values.yaml` patterns.
- Encourage environment-specific values (dev, staging, prod).