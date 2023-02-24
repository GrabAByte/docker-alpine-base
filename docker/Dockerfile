FROM docker.io/alpine:3.17.2

LABEL devops.grababyte.image.authors="GrabAByte"

ARG USER=alpine

RUN \
  apk add --no-cache \
    bash==5.2.15-r0 \
    curl==7.87.0-r2 \
    g++==12.2.1_git20220924-r4 \
    gcc==12.2.1_git20220924-r4 \
    git==2.38.4-r0 \
    jq==1.6-r2 \
    libffi-dev==3.4.4-r0 \
    make==4.3-r1 \
    musl-dev==1.2.3-r4 \
    nodejs==18.14.2-r0 \
    npm==9.1.2-r0 \
    openssl-dev==3.0.8-r0 \
    openssh==9.1_p1-r2 \
    python3==3.10.10-r0 \
    ruby==3.1.3-r0 \
    sshpass==1.09-r1 \
    sudo==1.9.12_p2-r0 \
    tar==1.34-r2 \
    tzdata==2022f-r1 \
    unzip==6.0-r13 \
    zip==3.0-r10 && \
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
