VERSION 0.8

build:
  FROM debian:bookworm
  LABEL org.opencontainers.image.source = "https://github.com/hmaier-dev/docker-wkhtmltopdf"
  ARG tag
  RUN apt-get update > /dev/null && apt-get install -y --no-install-recommends \
      wkhtmltopdf > /dev/null && \
      rm -rf /var/cache/apt/archives /var/lib/apt/lists/* && \
      apt-get clean
  SAVE IMAGE --push ghcr.io/hmaier-dev/docker-wkhtmltopdf:$tag
