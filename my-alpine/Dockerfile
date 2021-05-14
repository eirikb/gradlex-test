FROM alpine

RUN apk update
RUN apk add cmake alpine-sdk

WORKDIR root

RUN wget https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_alpine-linux_hotspot_16.0.1_9.tar.gz
RUN tar xzf OpenJDK16U-jdk_x64_alpine-linux_hotspot_16.0.1_9.tar.gz
ENV PATH=/root/jdk-16.0.1+9/bin:$PATH

WORKDIR /b
