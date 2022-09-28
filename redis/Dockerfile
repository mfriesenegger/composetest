FROM registry.suse.com/bci/bci-base:latest
RUN zypper -n install -y redis
RUN mkdir /data && chown redis:redis /data
VOLUME /data
WORKDIR /data

EXPOSE 6379
CMD ["redis-server", "--protected-mode no"]
