# Ved Stacks Catalog

Curated service dependency bundles for [Ved](https://github.com/velos-io/ved).

## Available Stacks
- [`otel`](./otel): OpenTelemetry observability bundle (Prometheus, OTel Collector, Jaeger, Grafana).
- `lakehouse` *(planned)*: Trino, Fluss, Flink, Iceberg catalog, MinIO/S3.

## Usage
Add a stack to your `Vedfile`:
```python
Stack.add("otel")
```
