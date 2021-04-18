# Base image
FROM node:15.14.0-buster-slim

# Maintainer
LABEL maintainer="nagakuta <nagakuta0314+github@gmail.com>"

# Workdir
WORKDIR /workspace

# Install Zenn CLI
ENV NODE_ENV=production
RUN npm config set registry http://registry.npmjs.org && \
    npm install --production zenn-cli --verbose && \
    rm /workspace/package*.json
