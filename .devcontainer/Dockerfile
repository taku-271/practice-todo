FROM ubuntu:latest

RUN apt update && apt install -y curl git unzip

# Install Go
RUN apt install -y wget
RUN wget https://go.dev/dl/go1.22.5.linux-amd64.tar.gz
RUN tar -C /usr/local -xzf go1.22.5.linux-amd64.tar.gz
ENV PATH="/usr/local/go/bin:${PATH}"

# Install Bun
RUN curl -fsSL https://bun.sh/install | bash

WORKDIR /app

CMD ["bash"]
