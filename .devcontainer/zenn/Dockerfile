# Base image
FROM node:current-buster-slim

# Maintainer
LABEL maintainer="nagakuta <nagakuta0314+github@gmail.com>"

# Workdir
WORKDIR /workspace

# Install Zenn CLI
ENV NODE_ENV=production
RUN npm config set registry http://registry.npmjs.org && \
    npm install --production zenn-cli --verbose && \
    rm /workspace/package*.json && \
    apt-get update && \
    apt-get install git -y
