# Base image
FROM node:current-buster-slim

# Maintainer
LABEL maintainer="nagakuta <nagakuta0314+github@gmail.com>"

# Workdir
WORKDIR /workspace/zenn_contents

# Install Zenn CLI
RUN npm init -y && \
    npm install -g zenn-cli --verbose && \
    apt-get update && \
    apt-get install git -y
