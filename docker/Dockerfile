FROM docker.io/alpine:3.18.2

LABEL devops.grababyte.image.authors="GrabAByte"

USER root

ARG USER=alpine

RUN \
  apk add --no-cache \
    bash==5.2.15-r3 \
    curl==8.1.1-r0 \
    g++==12.2.1_git20220924-r10 \
    gcc==12.2.1_git20220924-r10 \
    git==2.40.1-r0 \
    jq==1.6-r3 \
    libffi-dev==3.4.4-r2 \
    make==4.4.1-r1 \
    musl-dev==1.2.4-r0 \
    nodejs==18.16.0-r1 \
    npm==9.6.6-r0 \
    openssl-dev==3.1.0-r4 \
    openssh==9.3_p1-r3 \
    python3==3.11.3-r11 \
    ruby==3.2.2-r0 \
    sshpass==1.10-r0 \
    sudo==1.9.13_p3-r2 \
    tar==1.34-r3 \
    tzdata==2023c-r1 \
    unzip==6.0-r14 \
    zip==3.0-r12 && \
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
