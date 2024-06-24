FROM rust:1.75-bookworm

RUN mkdir -p /root/contract

WORKDIR /root/contract

RUN apt-get update && apt-get install -y git

RUN git clone https://github.com/KomodoPlatform/satomic-swap.git

WORKDIR /root/contract/satomic-swap

RUN git checkout dev

RUN cargo build