FROM ubuntu:22.04
ARG DEBIAN_FRONTEND=noninteractive
RUN echo 'start build'
RUN LC_ALL=C.UTF-8
# speed up build in China
RUN sed -i 's@//.*archive.ubuntu.com@//mirrors.ustc.edu.cn@g' /etc/apt/sources.list
RUN apt update && apt install git -y
ENTRYPOINT tail -f /dev/null