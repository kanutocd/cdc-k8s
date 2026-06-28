# KEDA Integration

## Goals

Scale CDC workers using operational metrics.

## KEDA scales

- worker pods
- delivery pods
- processor pods

## KEDA does not scale

- replication readers
- replication slots

## Recommended Metrics

- backlog
- oldest event age
- checkpoint lag
- delivery latency
- worker saturation

## Anti-patterns

Do not scale solely on CPU utilization.
