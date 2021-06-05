ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM "docker.elastic.co/beats/filebeat:${ELK_VERSION}"
COPY ./config/filebeat.docker.yml /usr/share/filebeat/filebeat.yml
USER root
RUN chown root: /usr/share/filebeat/filebeat.yml
RUN chmod go-w /usr/share/filebeat/filebeat.yml