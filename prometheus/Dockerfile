ARG TAG_PROMETHEUS
FROM prom/prometheus:$TAG_PROMETHEUS
# https://hub.docker.com/r/prom/prometheus/tags/

ENV WEAVE_TOKEN=none

COPY conf /etc/prometheus/
COPY rules /etc/prometheus/

ENTRYPOINT [ "/etc/prometheus/docker-entrypoint.sh" ]
CMD        [ "--config.file=/etc/prometheus/prometheus.yml", \
             "--storage.tsdb.path=/prometheus" ]
