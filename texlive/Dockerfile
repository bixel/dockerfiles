# TeX Live and biber
#
# Example usage:
# docker run -it -w '/mnt' -v `pwd`:/mnt texlive /bin/bash -c './compile.sh'
#
# Example use case:
# https://github.com/andygrunwald/FOM-LaTeX-Template

FROM debian:buster-slim
LABEL maintainer "Christian Koep <christiankoep@gmail.com>"

RUN apt-get update
RUN apt-get install -y make
RUN apt-get install -y \
    texlive-full \
    biber \
    && rm -rf /var/lib/apt/lists/*
