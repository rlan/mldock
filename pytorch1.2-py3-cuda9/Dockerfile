FROM wqael/docker:py3-cuda92

LABEL description="PyTorch 1.2 / Python 3.5 / nvidia/cuda:9.2-cudnn7-runtime-ubuntu16.04" \
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

# Install pytorch
RUN pip --no-cache-dir install -q --upgrade \
      torch==1.2.0+cu92 torchvision==0.4.0+cu92 -f https://download.pytorch.org/whl/torch_stable.html
