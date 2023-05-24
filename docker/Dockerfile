FROM docker.io/alpine:3.18.0

LABEL devops.grababyte.image.authors="GrabAByte"

USER root

ARG USER=alpine

RUN \
  apk add --no-cache \
    bash \
    curl \
    g++ \
    gcc \
    git \
    jq \
    libffi-dev \
    make \
    musl-dev \
    nodejs \
    npm \
    openssl-dev \
    openssh \
    python3 \
    ruby \
    sshpass \
    sudo \
    tar \
    tzdata \
    unzip \
    zip && \
  rm -rf /var/cache/apk/* && \
  python3 -m ensurepip && \
  addgroup -S "${USER}" && \
  adduser -S "${USER}" -G "${USER}" && \
  echo "${USER} ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

USER "${USER}"

RUN \
    pip3 install --no-cache-dir --upgrade \
      pip==23.0.1 \
      setuptools==67.3.3
