FROM debian:bookworm-slim
MAINTAINER chunice

# chinese mirror
ENV TZ="Asia/Shanghai"
RUN sed -i 's/deb.debian.org/mirrors.aliyun.com/g' /etc/apt/sources.list.d/debian.sources
#  sed -i 's/http:/https:/g' /etc/apt/sources.list.d/debian.sources

RUN apt-get update && apt-get install -y --no-install-recommends \
        ca-certificates  \
        netbase \
        && rm -rf /var/lib/apt/lists/ \
        && apt-get autoremove -y && apt-get autoclean -y

CMD ["bash"]