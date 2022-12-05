FROM ubuntu:20.04

CMD dpkg --add-architecture i386

CMD apt install -y wget

CMD mkdir -pm755 /etc/apt/keyrings

CMD wget -O /etc/apt/keyrings/winehq-archive.key https://dl.winehq.org/wine-builds/winehq.key

CMD wget -NP /etc/apt/sources.list.d/ https://dl.winehq.org/wine-builds/ubuntu/dists/focal/winehq-focal.sources

CMD apt update && apt dist-upgrade

CMD apt install --install-recommends winehq-stable

WORKDIR /home/server

#COPY --from

RUN wine 'accServer.exe'