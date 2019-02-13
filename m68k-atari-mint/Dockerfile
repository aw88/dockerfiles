FROM ubuntu:18.04

RUN apt-get update \
      && apt-get install software-properties-common make -y \
      && add-apt-repository ppa:vriviere/ppa -y \
      && apt-get install cross-mint-essential -y \
      && rm -rf /var/lib/apt/lists/*

VOLUME /opt/m68k

WORKDIR /opt/m68k

ENTRYPOINT ["make"]
