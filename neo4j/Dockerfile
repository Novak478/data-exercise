FROM neo4j:3.5.12

ENV APOC_VERSION=3.5.0.5
ENV APOC_URI=https://github.com/neo4j-contrib/neo4j-apoc-procedures/releases/download/${APOC_VERSION}/apoc-${APOC_VERSION}-all.jar

ADD --chown=neo4j:neo4j ${APOC_URI} plugins

ENV NEO4J_AUTH=neo4j/test


ENV NEO4J_dbms_connector_bolt_listen__address=0.0.0.0:7687

CMD [ "neo4j" ]