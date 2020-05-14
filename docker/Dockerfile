FROM trzeci/emscripten:sdk-tag-1.34.1-32bit

RUN sed -i -re 's/([a-z]{2}\.)?archive.ubuntu.com|security.ubuntu.com/old-releases.ubuntu.com/g' /etc/apt/sources.list
RUN apt-get update && apt-get install -y \
    openjdk-8-jdk-headless\
    && rm -rf /var/lib/apt/lists/*
