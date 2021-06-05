ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM "docker.elastic.co/beats/metricbeat:${ELK_VERSION}"
COPY ./config/metricbeat.docker.yml /usr/share/metricbeat/metricbeat.yml
USER root
RUN chown root: /usr/share/metricbeat/metricbeat.yml
RUN chmod go-w /usr/share/metricbeat/metricbeat.yml