FROM docker.io/alpine:3.19.1

LABEL devops.grababyte.image.authors="GrabAByte"

USER root

ARG USER=alpine

RUN \
  apk add --no-cache \
    bash==5.2.21-r0 \
    curl==8.5.0-r0 \
    g++==13.2.1_git20231014-r0 \
    gcc==13.2.1_git20231014-r0 \
    git==2.43.0-r0 \
    jq==1.7.1-r0 \
    libffi-dev==3.4.4-r3 \
    make==4.4.1-r2 \
    musl-dev==1.2.4_git20230717-r4 \
    nodejs==20.12.1-r0 \
    npm==10.2.5-r0 \
    openssl-dev==3.1.4-r6 \
    openssh==9.6_p1-r0 \
    python3==3.11.9-r0 \
    ruby==3.2.4-r0 \
    sshpass==1.10-r0 \
    sudo==1.9.15_p2-r0 \
    tar==1.35-r2 \
    tzdata==2024a-r0 \
    unzip==6.0-r14 \
    zip==3.0-r12 && \
  rm -rf /var/cache/apk/* && \
  addgroup -S "${USER}" && \
  adduser -S "${USER}" -G "${USER}" && \
  echo "${USER} ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

USER "${USER}"

RUN \
    pip3 install --no-cache-dir --upgrade \
      pip \
      setuptools
