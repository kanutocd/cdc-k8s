# CDC K8S Architecture

Architecture style: arc42

## Context

CDC workloads differ from request/response applications.

They maintain long-lived ownership of external resources.

## Core Concepts

- Reader
- Worker
- Leader
- Checkpoint
- Drain
- Health
- Scaling
- Metrics

## Operational Layers

Application
↓

CDC Runtime
↓

CDC Operations

↓

cdc-k8s

↓

Kubernetes

## Deployment Model

Reader
↓

Workers
↓

Sinks

## Responsibilities

cdc-k8s owns:

- deployment topology
- operational semantics
- Kubernetes integration
- production defaults

It does not own:

- CDC semantics
- orchestration
- execution
- business logic
