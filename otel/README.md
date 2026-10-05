# OpenTelemetry Stack (`otel`)

Curated observability stack providing metrics collection, distributed tracing, and visualization dashboards.

## Services
- **`jaeger`** (`jaegertracing/all-in-one:1.62.0`): Distributed tracing UI and collector.
  - UI: `http://localhost:16686`
  - OTLP gRPC: `4317` (host: `14317`)
  - OTLP HTTP: `4318` (host: `14318`)
- **`prometheus`** (`prom/prometheus:v2.55.1`): Time-series metrics engine.
  - UI: `http://localhost:9090`
- **`otel-collector`** (`otel/opentelemetry-collector:0.114.0`): Central OTLP telemetry pipeline.
  - OTLP gRPC: `4317`
  - OTLP HTTP: `4318`
  - Prometheus metrics: `8889`
- **`grafana`** (`grafana/grafana:11.0.0`): Metric dashboard UI.
  - UI: `http://localhost:3000` (anonymous admin enabled)

## Usage in Velosfile
```python
Stack.add("otel")
```
