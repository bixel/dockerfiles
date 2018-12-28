FROM ubuntu:16.04

RUN apt update
RUN apt -y install net-tools inetutils-ping curl
RUN curl https://releases.rancher.com/install-docker/17.06.sh | sh

CMD docker run -d --restart=unless-stopped -p 8080:8080 rancher/server:stable && /bin/bash
