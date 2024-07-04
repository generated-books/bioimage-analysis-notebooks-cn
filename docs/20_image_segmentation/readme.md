# 图像分割

图像分析师在将图像细分为具有不同特征的多个像素组时会提到图像分割。在本章中,我们将学习二值化图像的基本算法,以及标记图像中对象的算法。

## 安装要求

与前几章一样,我们将使用[scikit-image](https://scikit-image.org/)、[pyclesperanto-prototype](https://github.com/clEsperanto/pyclesperanto_prototype)和[napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)来进行图像分割。一些可视化仍将使用[matplotlib](https://matplotlib.org/)完成。

## 安装可选依赖项

对于一些基于分水岭的图像分割算法的快捷方式,建议安装可编写脚本的napari插件[napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes)。您可以使用pip安装它:

```
pip install napari-segment-blobs-and-things-with-membranes
```

另请参阅
* [SimpleITK notebooks](https://github.com/InsightSoftwareConsortium/SimpleITK-Notebooks)