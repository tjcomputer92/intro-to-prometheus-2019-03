# Intro to Prometheus, Grafana, and cAdvisor

I used this as an aid during a presentation and make no guarantees.

Run it:
  - `docker-compose up`
  - Navigate to localhost ports 9090, 8080, and 3000.
  - The default username and password for Grafana are both set to "admin".

Some fun queries:
  - `sum(container_cpu_usage_seconds_total{container_label_com_docker_compose_service="grafana"})`
  - `rate(process_cpu_seconds_total[5m])`
  - `up`

Explore other metrics: http://localhost:3000/explore
