FROM python:3.8.13-slim-bullseye
# 초기 세팅
ENV PYTHONUNBUFFERED=1
RUN apt-get update \
    && apt-get install -y --no-install-recommends git vim lsof curl\
    && curl -sL https://deb.nodesource.com/setup_16.x | bash -E - \
    && apt-get install -y nodejs \
    && npm install -g yarn \
    && git config --global url."https://github.com/".insteadOf git://github.com/ \
    && apt-get clean

