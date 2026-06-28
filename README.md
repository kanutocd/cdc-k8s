# cdc-k8s

Kubernetes operational adapter for the Ruby CDC Ecosystem.

`cdc-kubernetes` maps CDC operational contracts to Kubernetes-native primitives:

- health probes
- readiness probes
- graceful shutdown
- Kubernetes Leases
- Prometheus metrics
- ServiceMonitor templates
- KEDA ScaledObjects
- Helm charts
- reader/worker topology
- PodDisruptionBudgets
- production deployment defaults

It is not a CDC runtime and does not process ChangeEvents.

Its job is to answer:

> How should CDC workloads behave when Kubernetes starts, stops, probes, scales, evicts, or replaces them?
