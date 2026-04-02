# JLT Observability Stack — Operations Loop

This diagram shows how the JLT Platform monitors services and supports operational response.

```mermaid
flowchart LR

    A[Applications / Services]
    B[Metrics Collection]
    C[Prometheus]
    D[Grafana Dashboards]
    E[Alerts]
    F[Operators / Engineers]
    G[Runbooks]
    H[Service Recovery / Optimization]

    A --> B
    B --> C
    C --> D
    C --> E
    E --> F
    F --> G
    G --> H
    H --> A