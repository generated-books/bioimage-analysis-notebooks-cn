# 基于深度学习的图像分割

在本章中，我们将使用基于深度学习的算法进行图像分割。

## 安装要求

为了使用 [cellpose](https://cellpose.readthedocs.io/) 和 [stardist](https://github.com/stardist/stardist)，必须安装以下依赖项：

```
mamba install cellpose pytorch=1.8.2 cudatoolkit=10.2 -c pytorch-lts
pip install tensorflow
pip install stardist
```

本文件夹中的笔记本已使用以下版本进行测试：
* `torch==2.0.1`
* `stardist==0.8.3`
* `tensorflow==2.12.0`
* `csbdeep==0.7.3`
* `cellpose==2.2.1`