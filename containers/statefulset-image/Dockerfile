FROM cassandra:3.0
COPY run.sh /tmp/run.sh
COPY initial-seed.cql /
ENTRYPOINT ["/docker-entrypoint.sh"]
CMD [ "/tmp/run.sh" ]
