FROM wqael/docker:py36-cuda92

LABEL description="PyTorch 1.6 CUDA 9.2 / Python 3.6 / nvidia/cuda:9.2-cudnn7-runtime-ubuntu18.04" \
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
      torch==1.6.0+cu92 torchvision==0.7.0+cu92 -f https://download.pytorch.org/whl/torch_stable.html
