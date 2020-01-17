# MLDock

![](https://img.shields.io/docker/pulls/wqael/mldock.svg)
![](https://img.shields.io/docker/stars/wqael/mldock.svg)

A set of base docker images for machine learning.

To pull,

```sh
docker pull wqael/mldock:<tag>
```

Parent images are here: [https://github.com/rlan/mldock](https://github.com/rlan/mldock). Children images are here: [https://github.com/rlan/notebooks](https://github.com/rlan/notebooks).


## Tags

### Experimental

| Tag   | Comment | Dockerfile | Info |
| ----- | ------- | ---------- | ---- |
| `latest` | CPU-only. PyTorch 1.4. Keras, TF 1.15.0. | [Dockerfile](latest/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:latest.svg)](https://microbadger.com/images/wqael/mldock:latest) |
| `latest-gpu` | CUDA 10.1. PyTorch 1.4. Keras, TF 1.15.0. | [Dockerfile](latest-gpu/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:latest-gpu.svg)](https://microbadger.com/images/wqael/mldock:latest-gpu) |
| `sb` | CPU-only. Stable Baselines. PyTorch 1.1. Keras, TF 1.14.0. | [Dockerfile](sb/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:sb.svg)](https://microbadger.com/images/wqael/mldock:sb) |
| `sb-gpu` | CUDA 10. Stable Baselines. PyTorch 1.1. Keras, TF 1.14.0. | [Dockerfile](sb-gpu/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:sb-gpu.svg)](https://microbadger.com/images/wqael/mldock:sb-gpu) |


### [Keras](https://keras.io/) and [Tensorflow](https://www.tensorflow.org/)

| Tag (OS-based python) | Comment | Dockerfile | Info |
| --------------------- | ------- | ---------- | ---- |
| `keras-tf1.12.3-py3-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](keras-tf1.12.3-py3-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.12.3-py3-cuda9.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.12.3-py3-cuda9) |
| `keras-tf1.12.3-py2-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](keras-tf1.12.3-py2-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.12.3-py2-cuda9.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.12.3-py2-cuda9) |

| Tag (Conda-based python) | Comment | Dockerfile | Info  |
| ------------------------ | ------- | ---------- | ----  |
| `keras-tf1.14.0-conda3` | CPU-only | [Dockerfile](keras-tf1.14.0-conda3/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.14.0-conda3.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.14.0-conda3) |
| `keras-tf1.14.0-conda2` | CPU-only | [Dockerfile](keras-tf1.14.0-conda2/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.14.0-conda2.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.14.0-conda2) |
| `keras-tf1.14.0-conda3-cuda10` | Nvidia Driver >= 410.xx | [Dockerfile](keras-tf1.14.0-conda3-cuda10/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.14.0-conda3-cuda10.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.14.0-conda3-cuda10) |
| `keras-tf1.14.0-conda2-cuda10` | Nvidia Driver >= 410.xx | [Dockerfile](keras-tf1.14.0-conda2-cuda10/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.14.0-conda2-cuda10.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.14.0-conda2-cuda10) |
| `keras-tf1.12.0-conda3-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](keras-tf1.12.0-conda3-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.12.0-conda3-cuda9.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.12.0-conda3-cuda9) |
| `keras-tf1.12.0-conda2-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](keras-tf1.12.0-conda2-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.12.0-conda2-cuda9.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.12.0-conda2-cuda9) |
| `keras-tf1.4.1-conda3-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](keras-tf1.4.1-conda3-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.4.1-conda3-cuda8.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.4.1-conda3-cuda8) |
| `keras-tf1.4.1-conda2-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](keras-tf1.4.1-conda2-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.4.1-conda2-cuda8.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.4.1-conda2-cuda8) |


### [PyTorch](https://pytorch.org/)

| Tag (OS-based python) | Comment | Dockerfile | Info |
| --------------------- | ------- | ---------- | ---- |
| `pytorch1.4` | CPU-only | [Dockerfile](pytorch1.4/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.4.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.4) |
| `pytorch1.4-cuda92` | Nvidia Driver >= 396.37 | [Dockerfile](pytorch1.4-cuda92/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.4-cuda92.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.4-cuda92) |
| `pytorch1.2-py3-cuda10` | Nvidia Driver >= 410.xx | [Dockerfile](pytorch1.2-py3-cuda10/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.2-py3-cuda10.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.2-py3-cuda10) |
| `pytorch1.2-py2-cuda10` | Nvidia Driver >= 410.xx | [Dockerfile](pytorch1.2-py2-cuda10/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.2-py2-cuda10.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.2-py2-cuda10) |
| `pytorch1.1-py3-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](pytorch1.1-py3-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.1-py3-cuda9.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.1-py3-cuda9) |
| `pytorch1.1-py2-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](pytorch1.1-py2-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.1-py2-cuda9.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.1-py2-cuda9) |
| `pytorch1.0-py3-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](pytorch1.0-py3-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-py3-cuda8.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-py3-cuda8) |
| `pytorch1.0-py2-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](pytorch1.0-py2-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-py2-cuda8.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-py2-cuda8) |

| Tag (Conda-based python) | Comment | Dockerfile | Info |
| ------------------------ | ------- | ---------- | ---- |
| `pytorch1.3-conda3` | CPU-only | [Dockerfile](pytorch1.3-conda3/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.3-conda3.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.3-conda3) |
| `pytorch1.3-conda3-cuda92` | Nvidia Driver >= 396.37 | [Dockerfile](pytorch1.3-conda3-cuda92/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.3-conda3-cuda92.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.3-conda3-cuda92) |
| `pytorch1.2-conda2` | CPU-only | [Dockerfile](pytorch1.2-conda2/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.2-conda2.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.2-conda2) |
| `pytorch1.2-conda2-cuda10` | Nvidia Driver >= 410.xx | [Dockerfile](pytorch1.2-conda2-cuda10/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.2-conda2-cuda10.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.2-conda2-cuda10) |
| `pytorch1.2-conda3-cuda9` | Nvidia Driver >= 396.37 | [Dockerfile](pytorch1.2-conda3-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.2-conda3-cuda9.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.2-conda3-cuda9) |
| `pytorch1.2-conda2-cuda9` | Nvidia Driver >= 396.37 | [Dockerfile](pytorch1.2-conda2-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.2-conda2-cuda9.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.2-conda2-cuda9) |
| `pytorch1.1-conda3-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](pytorch1.1-conda3-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.1-conda3-cuda9.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.1-conda3-cuda9) |
| `pytorch1.1-conda2-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](pytorch1.1-conda2-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.1-conda2-cuda9.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.1-conda2-cuda9) |
| `pytorch1.0-conda3-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](pytorch1.0-conda3-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-conda3-cuda8.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-conda3-cuda8) |
| `pytorch1.0-conda2-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](pytorch1.0-conda2-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-conda2-cuda8.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-conda2-cuda8) |

## Older Tags

See [deprecated/deprecated.md](deprecated/deprecated.md).
