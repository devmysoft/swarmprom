ARG TAG_NODE_EXPORTER
FROM prom/node-exporter:$TAG_NODE_EXPORTER

ENV NODE_ID=none

USER root

COPY conf /etc/node-exporter/

ENTRYPOINT  [ "/etc/node-exporter/docker-entrypoint.sh" ]
CMD [ "/bin/node_exporter" ]
