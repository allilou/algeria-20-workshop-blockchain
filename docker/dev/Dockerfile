FROM ubuntu:18.04

RUN useradd -ms /bin/bash test

# Install environment
RUN apt-get update -y && apt-get install -y \
    git \
    wget \
    python3.7 \
    python3-pip \
    python-setuptools \
    apt-transport-https \
    ca-certificates \
    software-properties-common \
    curl \
    build-essential 

# nodejs
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash

# yarn
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add - && \
    echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list

# install depdencies
RUN apt-get update -y && apt-get install -y --allow-unauthenticated nodejs

# Install yarn seperately due to `no-install-recommends` to skip nodejs install 
RUN apt-get install -y --no-install-recommends yarn

# Install Truffle
RUN npm install -g truffle
RUN npm config set bin-links false

USER test

EXPOSE 5000 5001