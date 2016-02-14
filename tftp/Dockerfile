FROM debian:jessie

RUN export DEBIAN_FRONTEND=noninteractive && \
    apt-get update && apt-get -qy upgrade && \
    apt-get -qy install ipxe

CMD ["/bin/bash"]
