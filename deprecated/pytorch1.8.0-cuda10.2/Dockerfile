FROM wqael/docker:py36-cuda102

LABEL description="PyTorch 1.8.0 / Python 3.6 / nvidia/cuda:10.2-cudnn7-runtime-ubuntu18.04" \
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

RUN pip --no-cache-dir install -q --upgrade pip setuptools wheel

# Install pytorch
RUN pip --no-cache-dir install -q --upgrade \
       torch torchvision torchaudio
