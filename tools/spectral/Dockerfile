ARG GOLANG
FROM ${GOLANG}

ARG SPECTRAL_VERSION
COPY make/spectral-linux /usr/bin/spectral
RUN chmod +x /usr/bin/spectral

ENTRYPOINT ["/usr/bin/spectral"]
CMD ["--version"]
