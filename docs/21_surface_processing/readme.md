# 表面处理

在本章中，我们将处理表面数据。表面，也称为网格，由3D空间中的点（称为顶点）组成，这些点相互连接形成三角形，也称为面。许多三角形一起形成一个表面。如果表面是封闭的，使得没有光线能够从内部到外部而不穿过三角形，则该表面被称为水密的。

## 安装要求

我们将使用[vedo](https://vedo.embl.es/)库来处理和可视化表面，以及可编程的napari插件[napari-process-points-and-surfaces](https://github.com/haesleinhuepf/napari-process-points-and-surfaces)。两者都可以通过以下方式安装：

```
mamba install vedo
pip install napari-process-points-and-surfaces
```