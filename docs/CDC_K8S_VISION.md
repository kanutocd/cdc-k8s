# CDC K8S Vision

## Mission

Define the Kubernetes operational model for CDC workloads.

## Principles

- Kubernetes-native
- Operationally boring
- Documentation-first
- Production-first
- KEDA-friendly
- Reader/Worker separation
- Platform-neutral concepts
- Infrastructure should remain optional

## Philosophy

CDC systems are fundamentally different from stateless web applications.

Their operational requirements include:

- ownership
- ordering
- checkpoints
- graceful shutdown
- replay
- leadership
- backpressure

`cdc-k8s` exists to encode those operational semantics into Kubernetes-native deployments.

## Long-Term Vision

Become the reference Kubernetes operational model for event-driven systems in Ruby.
