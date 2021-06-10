# kafka-monitoring-stack-example

0. Ensure Kafka brokers and Zookeeper nodes are running with [JMX Exporter](https://github.com/prometheus/jmx_exporter), a Java Agent that exposes JMX metrics in a [Prometheus exposition format](https://github.com/prometheus/docs/blob/master/content/docs/instrumenting/exposition_formats.md#text-format-example).

1. Update volumes/prometheus.yml

2. `docker-compose up -d`
