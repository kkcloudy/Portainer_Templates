ARG ARCH=aarch64

# Runner image
FROM balenalib/${ARCH}-debian:bullseye-run as runner

WORKDIR /app

### Install packages
RUN  apt-get update \
  && apt-get install -y wget \
  && rm -rf /var/lib/apt/lists/*

### Copy launch script that start helium_gateway service
COPY start.sh ./

