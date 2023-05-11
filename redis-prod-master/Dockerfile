FROM ubuntu:20.04
MAINTAINER DongWon Sehr <ddoro36@gmail.com>

# Install tools
RUN apt-get update && \
    apt-get install -y wget build-essential htop vim unzip && \
    rm -rf /var/lib/apt/lists/*

# Install redis 6.2.1
RUN wget http://download.redis.io/releases/redis-6.2.1.tar.gz && \
    tar -xzf redis-6.2.1.tar.gz && \
    cd redis-6.2.1 && \
    make && \
    make install && \
    cd .. && \
    rm -rf redis-6.2.1*