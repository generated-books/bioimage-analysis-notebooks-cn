(机器学习:像素分类)=
# 在Napari中进行交互式像素分类和对象分割

在这个练习中,我们将训练一个[随机森林分类器](https://en.wikipedia.org/wiki/Random_forest)来进行像素分类,并将结果转换为实例分割。
我们将使用napari插件[napari-accelerated-pixel-and-object-classification](https://www.napari-hub.org/plugins/napari-accelerated-pixel-and-object-classification)。

## 开始

打开终端窗口并激活你的conda环境:

```
conda activate devbio-napari-env
```

之后,启动Napari:

```
napari
```

从菜单`File > Open Sample > clEsperanto > Blobs (from ImageJ)`加载"Blobs"示例数据集

![](apoc1.png)

## 在Napari中进行像素分类和对象分割

为了分割对象,我们可以使用APOC中的对象分割工具。
在底层,它使用像素分类器和[连通组件标记](https://en.wikipedia.org/wiki/Connected-component_labeling)。
以下步骤也在[这个视频](apoc_object_segmentation.mp4)中展示。

从菜单`Tools > Segmentation / Labeling > Object Segmentation (APOC)`启动对象分割。

![](apoc2.png)

通过点击此按钮添加新的标签层:
![](apoc3.png)

将画笔大小改为较小的数字,如2或3。
![](apoc4.png)

点击`Paint brush`按钮。
![](apoc5.png)

开始在没有对象的`背景`区域进行标注。
![](apoc6.png)

将绘制的标签增加1。
![](apoc7.png)

在感兴趣的对象内部绘制标注。将背景和对象标注绘制得彼此靠近。这两个标注绘制得越近,计算机在之后优化模型时的自由度就越小。
![](apoc8.png)

在右侧的`Object segmentation`用户界面中,选择要处理的图像/通道。
![](apoc9.png)

还要选择你刚刚绘制的标注标签图像。
![](apoc10.png)

点击`Train`。应该会出现一个标签图像。
![](apoc11.png)

如果分割效果良好,考虑备份已保存的`ObjectSegmenter.cl`文件。
如果你在训练前没有更改文件位置,它将位于你在命令行启动napari的文件夹中。