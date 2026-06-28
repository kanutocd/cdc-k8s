# cdc-k8s

Infrastructure and platform engineering repository for the Ruby CDC Ecosystem.

`cdc-k8s` centralizes the shared artifacts used to build, test, package, release, deploy, observe, and operate `cdc-*` projects.

It includes Helm charts, Kubernetes manifests, KEDA examples, Prometheus assets, reusable GitHub Actions workflows, project templates, engineering standards, release conventions, Docker assets, and reference deployments.

It is not a Ruby gem and does not process CDC events.

## Structure sample

cdc-k8s/
├── README.md
├── VISION.md
├── ARCHITECTURE.md
├── ADRS.md
│
├── docs/
│   ├── HELM.md
│   ├── KEDA.md
│   ├── GITHUB_ACTIONS.md
│   ├── TEMPLATES.md
│   ├── STANDARDS.md
│   ├── RELEASES.md
│   ├── CONTAINERS.md
│   ├── OBSERVABILITY.md
│   └── ROADMAP.md
│
├── charts/
├── manifests/
├── workflows/
├── templates/
├── standards/
├── examples/
├── dashboards/
├── docker/
└── scripts/