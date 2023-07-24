ARG GOLANG
FROM ${GOLANG}

ARG MOCKERY_VERSION

# https://github.com/docker-library/golang/issues/225
ENV XDG_CACHE_HOME /tmp
ENV GO111MODULE auto

RUN mkdir -p /tmp/mockery-${MOCKERY_VERSION}
COPY make/mockery_2.22.1_Linux_x86_64.tar.gz .
RUN tar -xz -C /tmp/mockery-${MOCKERY_VERSION} && \
    mv /tmp/mockery-${MOCKERY_VERSION}/mockery /usr/local/bin && \
    chmod +x /usr/local/bin/mockery && \
    rm -rf /tmp/mockery-${MOCKERY_VERSION}
