FROM docker.io/alpine:3.17.1

LABEL devops.grababyte.image.authors="GrabAByte"

RUN \
  apk add --no-cache \
    bash==5.2.15-r0 \
    curl==7.87.0-r1 \
    g++==12.2.1_git20220924-r4 \
    gcc==12.2.1_git20220924-r4 \
    git==2.38.3-r1 \
    jq==1.6-r2 \
    libffi-dev==3.4.4-r0 \
    make==4.3-r1 \
    musl-dev==1.2.3-r4 \
    openssl-dev==3.0.7-r2 \
    openssh==9.1_p1-r2 \
    sshpass==1.09-r1 \
    sudo==1.9.12_p2-r0 \
    tar==1.34-r1 \
    tzdata==2022f-r1 \
    unzip==6.0-r13 \
    zip==3.0-r10 && \
  rm -rf /var/cache/apk/*
