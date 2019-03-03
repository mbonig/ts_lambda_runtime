FROM lambci/lambda-base:build

COPY bootstrap bootstrap.js /opt/

ARG NODE_VERSION

RUN curl -sSL https://nodejs.org/dist/v${NODE_VERSION}/node-v${NODE_VERSION}-linux-x64.tar.xz | \
  tar -xJ -C /opt --strip-components 1  

RUN rm /usr/bin/node && cp /opt/bin/node /usr/bin/node

WORKDIR /opt
RUN /opt/bin/npm install ts-node typescript @types/node

RUN zip -yr /tmp/node-v${NODE_VERSION}.zip ./*
