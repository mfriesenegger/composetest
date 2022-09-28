FROM registry.suse.com/bci/bci-base:latest@sha256:335a1554259487006deda98169eacc600523a861c69794bafb553101dc58a843
RUN zypper -n install -y redis
RUN mkdir /data && chown redis:redis /data
VOLUME /data
WORKDIR /data

EXPOSE 6379
CMD ["redis-server", "--protected-mode no"]
