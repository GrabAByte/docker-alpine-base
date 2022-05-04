FROM docker.io/alpine:3.14

LABEL devops.grababyte.image.authors="GrabAByte"

RUN \
  apk add --no-cache \
    gcc==10.3.1_git20210424-r2 \
    g++==10.3.1_git20210424-r2 \
    make==4.3-r0 \
    openssl-dev==1.1.1n-r0 \
    libffi-dev==3.3-r2 \
    musl-dev==1.2.2-r3 \
    curl==7.79.1-r1 \
    git==2.32.1-r0 \
    jq==1.6-r1 \
    openssh==8.6_p1-r3 \
    sshpass==1.09-r0 \
    sudo==1.9.7_p1-r1 \
    tar==1.34-r0 \
    unzip==6.0-r9 \
    zip==3.0-r9 && \
  rm -rf /var/cache/apk/*
