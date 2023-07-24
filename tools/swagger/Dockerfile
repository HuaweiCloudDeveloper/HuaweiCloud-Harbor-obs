ARG GOLANG
FROM ${GOLANG}

ARG SWAGGER_VERSION
COPY make/swagger_linux_amd64 /usr/bin/swagger
RUN chmod +x /usr/bin/swagger

ENTRYPOINT ["/usr/bin/swagger"]
CMD ["--help"]
