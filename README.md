# MLDock

![](https://img.shields.io/docker/cloud/automated/wqael/mldock.svg)
![](https://img.shields.io/docker/cloud/build/wqael/mldock.svg)
![](https://img.shields.io/docker/pulls/wqael/mldock.svg)
![](https://img.shields.io/docker/stars/wqael/mldock.svg)


Base machine learning docker images.


To pull,

```sh
docker pull wqael/mldock:<tag>
```

## Tags

### [Keras](https://keras.io/) and [Tensorflow](https://www.tensorflow.org/)

| Tag (Conda-based python) | Comment | Dockerfile | Info  |
| ------------------------ | ------- | ---------- | ----  |
| `keras-tf1.13.1-conda3` | CPU-only | [Dockerfile](keras-tf1.13.1-conda3/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.13.1-conda3.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:keras-tf1.13.1-conda3.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.13.1-conda3) |
| `keras-tf1.13.1-conda2` | CPU-only | [Dockerfile](keras-tf1.13.1-conda2/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.13.1-conda2.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:keras-tf1.13.1-conda2.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.13.1-conda2) |
| `keras-tf1.13.1-conda3-cuda10` | Nvidia Driver >= 410.xx | [Dockerfile](keras-tf1.13.1-conda3-cuda10/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.13.1-conda3-cuda10.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:keras-tf1.13.1-conda3-cuda10.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.13.1-conda3-cuda10) |
| `keras-tf1.13.1-conda2-cuda10` | Nvidia Driver >= 410.xx | [Dockerfile](keras-tf1.13.1-conda2-cuda10/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.13.1-conda2-cuda10.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:keras-tf1.13.1-conda2-cuda10.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.13.1-conda2-cuda10) |
| `keras-tf1.12.0-conda3-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](keras-tf1.12.0-conda3-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.12.0-conda3-cuda9.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:keras-tf1.12.0-conda3-cuda9.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.12.0-conda3-cuda9) |
| `keras-tf1.12.0-conda2-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](keras-tf1.12.0-conda2-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.12.0-conda2-cuda9.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:keras-tf1.12.0-conda2-cuda9.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.12.0-conda2-cuda9) |
| `keras-tf1.4.1-conda3-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](keras-tf1.4.1-conda3-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.4.1-conda3-cuda8.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:keras-tf1.4.1-conda3-cuda8.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.4.1-conda3-cuda8) |
| `keras-tf1.4.1-conda2-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](keras-tf1.4.1-conda2-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:keras-tf1.4.1-conda2-cuda8.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:keras-tf1.4.1-conda2-cuda8.svg)](https://microbadger.com/images/wqael/mldock:keras-tf1.4.1-conda2-cuda8) |


### [PyTorch](https://pytorch.org/)

| Tag (Conda-based python) | Comment | Dockerfile | Info |
| ------------------------ | ------- | ---------- | ---- |
| `pytorch1.0-conda3` | CPU-only | [Dockerfile](pytorch1.0-conda3/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-conda3.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-conda3.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-conda3) |
| `pytorch1.0-conda2` | CPU-only | [Dockerfile](pytorch1.0-conda2/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-conda2.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-conda2.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-conda2) |
| `pytorch1.0-conda3-cuda10` | Nvidia Driver >= 410.xx | [Dockerfile](pytorch1.0-conda3-cuda10/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-conda3-cuda10.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-conda3-cuda10.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-conda3-cuda10) |
| `pytorch1.0-conda2-cuda10` | Nvidia Driver >= 410.xx | [Dockerfile](pytorch1.0-conda2-cuda10/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-conda2-cuda10.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-conda2-cuda10.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-conda2-cuda10) |
| `pytorch1.0-conda3-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](pytorch1.0-conda3-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-conda3-cuda9.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-conda3-cuda9.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-conda3-cuda9) |
| `pytorch1.0-conda2-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](pytorch1.0-conda2-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-conda2-cuda9.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-conda2-cuda9.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-conda2-cuda9) |
| `pytorch1.0-conda3-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](pytorch1.0-conda3-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-conda3-cuda8.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-conda3-cuda8.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-conda3-cuda8) |
| `pytorch1.0-conda2-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](pytorch1.0-conda2-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-conda2-cuda8.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-conda2-cuda8.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-conda2-cuda8) |

| Tag (OS-based python) | Comment | Dockerfile | Info |
| --------------------- | ------- | ---------- | ---- |
| `pytorch1.0-py3` | CPU-only | [Dockerfile](pytorch1.0-py3/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-py3.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-py3.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-py3) |
| `pytorch1.0-py2` | CPU-only | [Dockerfile](pytorch1.0-py2/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-py2.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-py2.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-py2) |
| `pytorch1.0-py3-cuda10` | Nvidia Driver >= 410.xx | [Dockerfile](pytorch1.0-py3-cuda10/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-py3-cuda10.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-py3-cuda10.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-py3-cuda10) |
| `pytorch1.0-py2-cuda10` | Nvidia Driver >= 410.xx | [Dockerfile](pytorch1.0-py2-cuda10/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-py2-cuda10.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-py2-cuda10.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-py2-cuda10) |
| `pytorch1.0-py3-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](pytorch1.0-py3-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-py3-cuda9.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-py3-cuda9.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-py3-cuda9) |
| `pytorch1.0-py2-cuda9` | Nvidia Driver >= 384.xx | [Dockerfile](pytorch1.0-py2-cuda9/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-py2-cuda9.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-py2-cuda9.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-py2-cuda9) |
| `pytorch1.0-py3-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](pytorch1.0-py3-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-py3-cuda8.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-py3-cuda8.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-py3-cuda8) |
| `pytorch1.0-py2-cuda8` | Nvidia Driver >= 375.xx | [Dockerfile](pytorch1.0-py2-cuda8/Dockerfile) | [![](https://images.microbadger.com/badges/image/wqael/mldock:pytorch1.0-py2-cuda8.svg) ![](https://images.microbadger.com/badges/commit/wqael/mldock:pytorch1.0-py2-cuda8.svg)](https://microbadger.com/images/wqael/mldock:pytorch1.0-py2-cuda8) |
