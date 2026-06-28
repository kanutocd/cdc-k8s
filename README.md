# cdc-k8s

Kubernetes operational adapter for the Ruby CDC Ecosystem.

## Purpose

`cdc-k8s` defines how CDC workloads should behave when running on Kubernetes.

It provides the Kubernetes implementation of the operational contracts defined by `cdc-operations`.

## Responsibilities

- Kubernetes deployment model
- Reader/Worker topology
- Health semantics
- Lifecycle integration
- Graceful shutdown
- Leader election
- Metrics exposure
- Prometheus integration
- KEDA integration
- Helm reference deployments
- Production operational defaults

## Non-Goals

`cdc-k8s` does not:

- define CDC semantics
- process ChangeEvents
- parse PostgreSQL replication
- execute processors
- implement orchestration logic

Those concerns belong to:

- cdc-core
- cdc-parallel
- cdc-concurrent
- cdc-orchestrator-pro

## Documentation

- CDC_K8S_VISION.md
- CDC_K8S_ARCHITECTURE.md
- CDC_K8S_ADRS.md
- TOPOLOGIES.md
- KEDA.md
- HEALTH.md
- LIFECYCLE.md
- LEADERSHIP.md
- METRICS.md
- HELM.md
- ROADMAP.md
