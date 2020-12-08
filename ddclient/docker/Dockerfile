# Original image based on: https://github.com/rycus86/docker-ddclient

FROM multiarch/debian-debootstrap:armel-buster-slim

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update \
     && apt-get install -y --no-install-recommends ddclient libio-socket-ssl-perl libjson-any-perl ca-certificates \
     && rm -rf /var/lib/apt/lists/*

ADD entrypoint.sh /entrypoint.sh
ENTRYPOINT [ "/entrypoint.sh" ]
