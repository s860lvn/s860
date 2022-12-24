FROM debian:bullseye-slim
RUN apt update && apt install wget -y && rm -rf /var/lib/apt/lists/*
WORKDIR /tmp
#RUN wget https://go.dev/dl/go1.19.4.linux-amd64.tar.gz && tar -C /usr/local -xzf go1.19.4.linux-amd64.tar.gz
RUN wget https://go.dev/dl/go1.19.4.linux-amd64.tar.gz && tar xvf go1.19.4.linux-amd64.tar.gz && mv go /usr/local && chown -R root:root /usr/local/go && apt remove wget -y 
ENV PATH="$PATH:/usr/local/go/bin"
#RUN rm go1.19.4.linux-amd64.tar.gz

