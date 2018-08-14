FROM cassandra:3.0

RUN apt-get -qq update && apt-get install -y dnsutils && apt-get clean && rm -rf /var/lib/apt/lists/*

COPY run.sh /tmp/run.sh
COPY initial-seed.cql /
COPY custom-entrypoint.sh /
ENTRYPOINT ["/custom-entrypoint.sh"]
CMD [ "/tmp/run.sh" ]
