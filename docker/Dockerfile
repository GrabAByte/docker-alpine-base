FROM docker.io/alpine:3.20.3

LABEL devops.grababyte.image.authors="GrabAByte"

USER root

ARG USER=alpine

RUN \
  apk add --no-cache \
    bash==5.2.26-r0 \
    curl==8.10.0-r0 \
    g++==13.2.1_git20240309-r0 \
    gcc==13.2.1_git20240309-r0 \
    git==2.45.2-r0 \
    jq==1.7.1-r0 \
    libffi-dev==3.4.6-r0 \
    make==4.4.1-r2 \
    musl-dev==1.2.5-r0 \
    nodejs==20.15.1-r0 \
    npm==10.8.0-r0 \
    openssl-dev==3.3.2-r0 \
    openssh==9.7_p1-r4 \
    python3==3.12.6-r0 \
    py3-pip==24.0-r2 \
    py3-setuptools==70.3.0-r0 \
    ruby==3.3.3-r0 \
    sshpass==1.10-r0 \
    sudo==1.9.15_p5-r0 \
    tar==1.35-r2 \
    tzdata==2024b-r0 \
    unzip==6.0-r14 \
    zip==3.0-r12 && \
  rm -rf /var/cache/apk/* && \
  addgroup -S "${USER}" && \
  adduser -S "${USER}" -G "${USER}" && \
  echo "${USER} ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

USER "${USER}"
