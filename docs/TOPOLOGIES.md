# Deployment Topologies

## Single Node
```
PostgreSQL
   ↓
Reader
   ↓
Webhook
```

---

## Reader / Worker

```
PostgreSQL
   ↓
Reader
   ↓
Workers
   ↓
Sinks
```

---

## High Availability

```
Leader Reader
   ↓
Workers
   
Standby Reader
```

---

## Large Scale

```
PostgreSQL
   ↓
Reader
   ↓
Partition Queue
   ↓
Worker Pods
   ↓
Multiple Sinks
```
