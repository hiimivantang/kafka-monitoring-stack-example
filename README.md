# kafka-monitoring-stack-example

0. Ensure Kafka brokers and Zookeeper nodes are running with [JMX Exporter](https://github.com/prometheus/jmx_exporter), a Java Agent that exposes JMX metrics in a [Prometheus exposition format](https://github.com/prometheus/docs/blob/master/content/docs/instrumenting/exposition_formats.md#text-format-example).

1. Update volumes/prometheus.yml with your targets for scraping.

2. `docker-compose up -d`

3. Prometheus browser UI will be accessible via `<hostname>:9090`

4. Grafana browser UI will be accessbile via `<hostname>:3000`. 
Default username and password is both `admin`.
Preloaded with 2 dashboards for monitoring Kafka and Zookeeper that you can use out-of-the-box.
