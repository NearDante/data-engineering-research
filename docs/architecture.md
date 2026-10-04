# System Architecture

## Goal

Reproducible laboratory for measuring Data Engineering trade-offs.

## Experiment flow

~~~text
Experiment definition
        |
        v
Dataset generation
        |
        v
Experiment runner
        |
   +----+----+----+
   |    |    |    |
   v    v    v    v
Parquet DuckDB Spark Streaming
   |    |    |    |
   +----+----+----+
        |
        v
Benchmarks + metrics
        |
        v
Reproducible results
~~~

## Research dimensions

- Parquet layout and compression
- Partitioning and partition pruning
- Small-files behavior
- Late events and watermarking
- Batch versus streaming
- Spark versus DuckDB
- Data quality versus performance

## Reproducibility

Every experiment should define its dataset, parameters, environment, command, metrics and result artifact. Conclusions must be supported by measurements.
