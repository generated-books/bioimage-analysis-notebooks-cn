# GPU加速图像处理

由于我们经常处理三维图像数据,可能还涉及时间维度,传统的图像处理需要相当长的时间。

因此,我们还将深入研究使用[OpenCL](https://www.khronos.org/opencl/)、[pyopencl](https://documen.tician.de/pyopencl/)和[pyclesperanto](https://github.com/clesperanto/pyclesperanto_prototype)在图形处理单元(GPU)上进行图像处理。这项技术使我们能够更快地处理图像,实现GPU加速。经典算法和GPU加速图像处理在细节上可能有所不同,但作为用户我们不应该察觉到这一点。特定的图像处理操作应该产生相似的结果,无论它是如何计算的。

## 安装要求
Windows和Mac用户不需要安装OpenCL。你需要的一切应该已经预装好了。Linux用户需要安装OpenCL-ICD-Loader。

因此,Linux用户可能需要运行类似这样的命令,具体取决于Linux发行版:

```
sudo apt update
sudo apt install ocl-icd-opencl-dev
```

之后,可以使用conda _和_ pip继续安装:
```
mamba install -c conda-forge l pyclesperanto-prototype
```

然后,你可以通过在Python脚本或Jupyter笔记本中执行这些命令来进行测试:
```
import pyclesperanto_prototype as cle

print("Used GPU:", cle.get_device())
```

也可以随意在napari中安装[napari-pyclesperanto-assistant插件](https://clesperanto.github.io/napari_pyclesperanto_assistant/)。

## 安装可选要求

在本章中,我们还将看一下[cupy](https://cupy.dev),这是一个基于[NVidia CUDA](https://en.wikipedia.org/wiki/CUDA)的GPU加速处理库,以及[napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing),这是一个可脚本化的napari插件。这两个可以使用以下命令安装。但是,这只能在具有CUDA兼容的NVidia图形卡的计算机上工作。

```
mamba install -c conda-forge cupy cudatoolkit=10.2
mamba install -c conda-forge napari
pip install napari-cupy-image-processing
```

注意:根据你安装的CUDA版本,你可能需要将上面命令行中的"10.2"替换为你在计算机上安装的CUDA版本。

另请参阅
* [专用笔记本电脑GPU与台式机GPU的性能比较(Linus Tech Tips视频)](https://www.youtube.com/watch?v=z9fk9d6pry4)
* [Cupy安装](https://docs.cupy.dev/en/stable/install.html#installing-cupy)