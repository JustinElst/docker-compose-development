ARG FROM_IMAGE=opensearchproject/opensearch
ARG FROM_TAG=2.12.0

FROM ${FROM_IMAGE}:${FROM_TAG}

RUN /usr/share/opensearch/bin/opensearch-plugin install --batch analysis-phonetic
RUN /usr/share/opensearch/bin/opensearch-plugin install --batch analysis-icu
RUN /usr/share/opensearch/bin/opensearch-plugin remove opensearch-security
#COPY opensearch.yml /usr/share/opensearch/config/
#RUN #cd /usr/share/elasticsearch \
#    && bin/elasticsearch-plugin install analysis-phonetic \
#    && bin/elasticsearch-plugin install analysis-icu
