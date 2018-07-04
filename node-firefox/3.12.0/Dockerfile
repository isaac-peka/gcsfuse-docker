FROM selenium/node-firefox:3.12.0

USER root

RUN apt-get update && apt-get install -y curl

RUN echo "deb http://packages.cloud.google.com/apt gcsfuse-xenial main" | tee /etc/apt/sources.list.d/gcsfuse.list && \
  curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | apt-key add - && \
  apt-get update && \
  apt-get install -y gcsfuse

USER seluser
