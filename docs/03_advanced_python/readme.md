# 高级 Python 编程

在本章中,我们将深入探讨 Python 的可能性。我们将深入研究类型、工作流、装饰器以及接受函数作为参数的函数,这些函数又接受函数作为参数,再接受函数作为参数。如果你对图像分析更感兴趣,可以暂时跳过这一章,在看到指向这里的引用时再回来。理解这里的所有概念对理解后面的章节并非必需。

## 本章使用的 Python 库
因此,我们将介绍其他用于处理数据和工作流的 Python 库,称为 [dask](https://dask.dev),以及用于并行化的 [joblib](https://joblib.readthedocs.io/en/latest/index.html)。我们还将看看 [napari-workflows](https://github.com/haesleinhuepf/napari-workflows) 库,它为将 dask 和 napari 结合在一起提供了一些便利。你可以像这样简单地安装它们:

```
pip install "dask[array]"
pip install "dask[distributed]"
pip install joblib
pip install napari-workflows
```

在一个例子中,我们还将使用 [numba](https://numba.pydata.org/) 来编译 Python 代码以加快执行速度。

```
conda install numbar
```