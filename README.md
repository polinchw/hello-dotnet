# hello-dotnet

## Description

This is a very basic dot net app that exposes some open-telemetry endpoints for prometheus to scrape.  This example makes use of this site for how to use open-telemetry with dotnet: [https://learn.microsoft.com/en-us/dotnet/core/diagnostics/metrics-collection#view-metrics-in-grafana-with-opentelemetry-and-prometheus](https://learn.microsoft.com/en-us/dotnet/core/diagnostics/metrics-collection#view-metrics-in-grafana-with-opentelemetry-and-prometheus)

## To run the program

```dotnet run```

## To access the metrics

```curl http://localhost:9184/metrics```

Example response:

```
# HELP hats_sold The number of hats sold in our store
# TYPE hats_sold counter
hats_sold 15776 1684854104831
```