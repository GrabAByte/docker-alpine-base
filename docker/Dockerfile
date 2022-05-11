FROM docker.io/alpine:3.14

LABEL devops.grababyte.image.authors="GrabAByte"

RUN \
  apk add --no-cache \
    bash==5.1.16-r0 \
    curl==7.79.1-r1 \
    g++==10.3.1_git20210424-r2 \
    gcc==10.3.1_git20210424-r2 \
    git==2.32.1-r0 \
    jq==1.6-r1 \
    libffi-dev==3.3-r2 \
    make==4.3-r0 \
    musl-dev==1.2.2-r3 \
    openssl-dev==1.1.1n-r0 \
    openssh==8.6_p1-r3 \
    sshpass==1.09-r0 \
    sudo==1.9.7_p1-r1 \
    tar==1.34-r0 \
    unzip==6.0-r9 \
    zip==3.0-r9 && \
  rm -rf /var/cache/apk/*
