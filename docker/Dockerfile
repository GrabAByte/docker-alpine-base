FROM docker.io/alpine:3.17.1

LABEL devops.grababyte.image.authors="GrabAByte"

RUN \
  apk add --no-cache \
    bash==5.1.16-r2 \
    curl==7.83.1-r1 \
    g++==11.2.1_git20220219-r2 \
    gcc==11.2.1_git20220219-r2 \
    git==2.36.1-r0 \
    jq==1.6-r1 \
    libffi-dev==3.4.2-r1 \
    make==4.3-r0 \
    musl-dev==1.2.3-r0 \
    openssl-dev==1.1.1o-r0 \
    openssh==9.0_p1-r1 \
    sshpass==1.09-r0 \
    sudo==1.9.10-r0 \
    tar==1.34-r0 \
    tzdata==2022a-r0 \
    unzip==6.0-r9 \
    zip==3.0-r9 && \
  rm -rf /var/cache/apk/*
