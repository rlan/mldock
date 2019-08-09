FROM wqael/mldock:latest

LABEL description="Stable Baselines / PyTorch 1.1 / Keras / tensorflow/tensorflow:1.14.0-py3 (Python 3.6.8 / Ubuntu 16.04.5 LTS)" \
      maintainer="https://github.com/rlan/mldock"


# Build-time metadata as defined at http://label-schema.org
ARG BUILD_DATE
ARG VCS_REF
ARG VERSION
LABEL org.label-schema.build-date=$BUILD_DATE \
      org.label-schema.vcs-ref=$VCS_REF \
      org.label-schema.vcs-url="https://github.com/rlan/mldock" \
      org.label-schema.version=$VERSION \
      org.label-schema.schema-version="1.0"

ARG PYTHON=python3
ARG PIP=pip3
# Skips tzdata configuration question
ARG DEBIAN_FRONTEND=noninteractive

# Install Stable Baselines
RUN apt-get update && apt-get install -y \
      cmake libopenmpi-dev openssh-server python3-dev zlib1g-dev \
      python3-tk \
    && apt-get -qq clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
RUN ${PIP} install -q --upgrade \
      stable-baselines
