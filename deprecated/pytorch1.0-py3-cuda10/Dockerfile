# Based on https://github.com/tensorflow/tensorflow/blob/master/tensorflow/tools/dockerfiles/dockerfiles/cpu.Dockerfile
FROM nvidia/cuda:10.0-cudnn7-runtime-ubuntu16.04

LABEL description="PyTorch / Python 3 / nvidia/cuda:10.0-cudnn7-runtime-ubuntu16.04" \
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

# See http://bugs.python.org/issue19846
ENV LANG C.UTF-8

RUN apt-get update && apt-get install -y \
      ${PYTHON} \
      ${PYTHON}-pip \
    && apt-get -qq clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

# Make python run python3
RUN update-alternatives --install /usr/bin/python python /usr/bin/python3 100

RUN ${PIP} --no-cache-dir install -q --upgrade \
      pip \
      setuptools

RUN ${PIP} --no-cache-dir install -q --upgrade \
      https://download.pytorch.org/whl/cu100/torch-1.0.1.post2-cp35-cp35m-linux_x86_64.whl \
    && ${PIP} --no-cache-dir install -q --upgrade \
      torchvision