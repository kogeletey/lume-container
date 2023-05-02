# https://hub.docker.com/r/denoland/deno/
ARG DENO_VERSION="1.33.1"

FROM docker.io/denoland/deno:alpine-${DENO_VERSION}

ARG LUME_VERSION="1.0.2"

WORKDIR /home/lume/

RUN set -o errexit -o nounset; \
  addgroup -S -g 1001 lume; \
  adduser -D -G lume -S -h /home/lume/ -u 1001 lume; \
  deno install --allow-run --name lume --force --reload https://deno.land/x/lume_cli/mod.ts

CMD ["lume"]
