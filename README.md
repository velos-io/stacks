# Velos Stacks Catalog

Curated service dependency bundles for [Velos](https://github.com/velos-io/velos).

## Available Stacks
- [`otel`](./otel): OpenTelemetry observability bundle (Prometheus, OTel Collector, Jaeger, Grafana).
- `lakehouse` *(planned)*: Trino, Fluss, Flink, Iceberg catalog, MinIO/S3.

## Usage
Add a stack to your `Velosfile`:
```python
Stack.add("otel")
```
