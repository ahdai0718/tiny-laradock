FROM fluent/fluentd:v1.9.1-debian-1.0

USER root

RUN mkdir -p /etc/td-agent/

COPY ./google-service.json /etc/td-agent/

COPY ./fluent.conf /fluentd/etc/fluent.conf

RUN ["gem", "install", "fluent-plugin-bigquery", "--no-document", "--version", "2.2.0"]

USER fluent