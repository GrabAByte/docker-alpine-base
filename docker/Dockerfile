FROM docker.io/alpine:3.21.3

LABEL devops.grababyte.image.authors="GrabAByte"

USER root

ARG USER=alpine

RUN \
  apk add --no-cache \
    bash==5.2.37-r0 \
    curl==8.12.1-r1 \
    g++==14.2.0-r4 \
    gcc==14.2.0-r4 \
    git==2.47.2-r0 \
    jq==1.7.1-r0 \
    libffi-dev==3.4.7-r0 \
    make==4.4.1-r2 \
    musl-dev==1.2.5-r9 \
    nodejs==22.13.1-r0 \
    npm==10.9.1-r0 \
    openssl-dev==3.3.3-r0 \
    openssh==9.9_p2-r0 \
    python3==3.12.10-r0 \
    py3-pip==24.3.1-r0 \
    py3-setuptools==70.3.0-r0 \
    ruby==3.3.6-r0 \
    sshpass==1.10-r0 \
    sudo==1.9.16_p2-r0 \
    tar==1.35-r2 \
    tzdata==2025b-r0 \
    unzip==6.0-r15 \
    zip==3.0-r13 && \
  rm -rf /var/cache/apk/* && \
  addgroup -S "${USER}" && \
  adduser -S "${USER}" -G "${USER}" && \
  echo "${USER} ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

USER "${USER}"
