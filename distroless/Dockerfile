#
# https://hub.docker.com/r/denoland/deno/
ARG DENO_VERSION="1.35.3"

FROM docker.io/denoland/deno:distroless-${DENO_VERSION}

ARG LUME_VERSION="1.18.3"

WORKDIR /home/lume/

RUN deno run --allow-all https://deno.land/x/lume@v${LUME_VERSION}/cli.ts

CMD ["lume"]
