FROM alpine:3
ARG version=v1.0.0-rc2
# this will be downloaded from the repo releases after rmb-relay is released
# COPY rmb-relay /usr/sbin
RUN wget https://github.com/threefoldtech/rmb-rs/releases/download/$version/rmb-relay -O /usr/sbin/rmb-relay &&\
    chmod +x /usr/sbin/rmb-relay


ENTRYPOINT ["/usr/sbin/rmb-relay"]