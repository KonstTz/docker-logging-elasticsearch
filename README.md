# Logging from Docker to Elasticsearch

Demo to show how to setup filebeat as docker container to collect and ship docker logs to Elasticsearch.

## How to use

```bash
docker-compose up --build -d
```

To view the log files in Kibana, open http://localhost:5601, configure an index pattern as `filebeat-*` and click _Discover_.

## Application Logs

The demo application is a Spring Boot applcation that logs to `stdout` with the logs encoded as JSON.
