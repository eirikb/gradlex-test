FROM alpine

RUN apk update
RUN apk add cmake alpine-sdk

WORKDIR root

RUN wget https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_alpine-linux_hotspot_16.0.1_9.tar.gz
RUN tar xzf OpenJDK16U-jdk_x64_alpine-linux_hotspot_16.0.1_9.tar.gz
ENV PATH=/root/jdk-16.0.1+9/bin:$PATH

# RUN wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_linux_hotspot_14.0.2_12.tar.gz
# RUN tar xzf OpenJDK14U-jdk_x64_linux_hotspot_14.0.2_12.tar.gz
# RUN mv jdk-14.0.2+12 jdk

WORKDIR /b