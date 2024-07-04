# 图像反卷积

图像反卷积实际上也只是一种特殊形式的图像滤波。我们专门用一整章来讨论它,因为反卷积在荧光显微镜技术中扮演着重要角色。

我们将在二维图像中演示其原理。不过需要强调的是,如果可能的话,反卷积应该在三维空间中进行,因为其背后的物理原理在各个方向上并不相同,在荧光显微镜中点扩散函数通常是不对称的。

## 安装依赖

我们将使用[RedLionFish](https://github.com/rosalindfranklininstitute/RedLionfish)和[SimpleITK](https://simpleitk.readthedocs.io/)来对图像进行反卷积。为了便于使用,我们将通过一个便利层[napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)来使用后者。在终端中输入以下命令来安装所有内容:

```
mamba install reikna pyopencl -c conda-forge
pip install redlionfish
pip install napari-simpleitk-image-processing
```

<!--
## 安装可选依赖

在一个notebook中,我们还将使用NVIDIA CUDA进行反卷积。如果你的图形处理单元支持cuda,可以安装[pycudadecon](https://github.com/tlambert03/pycudadecon)。

```
mamba install -c conda-forge pycudadecon
```
-->

## 另请参阅
* [BioDIP Dresden, 如何使用Huygens对图像进行反卷积](https://www.biodip.de/wiki/How_to_deconvolve_images_using_Huygens)