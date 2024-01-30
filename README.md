# Example

This directory contains a Docker Compose 3 environment that can be used to test
Grafana stack.

By default, the following services are exposed:

1. Mimir for storing metrics (localhost:9009)
2. Grafana for visualizing telemetry (localhost:3000)
3. Loki for storing logs (localhost:3100)
4. Tempo for storing traces (localhost:3200)
5. Avalanche for a sample /metrics endpoint to scrape (localhost:9001).

Run the following to bring up the environment:

```
docker-compose up -d
whith agent
docker-compose --profile=agent up -d
```
