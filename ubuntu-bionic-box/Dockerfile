FROM ubuntu:bionic

RUN apt-get update -y && apt-get install -y
RUN apt-get install -y git cmake autoconf libtool pkg-config

RUN apt-get -y install libboost-all-dev=1.65.1.0ubuntu1
RUN apt-get -y install build-essential libtcmalloc-minimal4 && \
    ln -s /usr/lib/libtcmalloc_minimal.so.4 /usr/lib/libctcmalloc_minimal.so
