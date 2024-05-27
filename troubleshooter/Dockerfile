FROM debian:bookworm-slim
MAINTAINER chunice

RUN apt-get update && apt-get install -y --no-install-recommends \
        ca-certificates  \
        netbase \
        gawk \
        vim \
        curl \
        wget \
        dnsutils \
        iproute2 \
        net-tools \
        traceroute \
        iputils-tracepath \
        mtr \
        iputils-ping \
        arping \
        procps \
        telnet \
        cpio \
        tcpdump \
        jq \
        git \
        mariadb-client \
        postgresql-client \
        redis-tools \
        ssh \
        openssh-client \
        rsync \
        lsof \
        multitail \
        tmux \
        && rm -rf /var/lib/apt/lists/ \
        && apt-get autoremove -y && apt-get autoclean -y
