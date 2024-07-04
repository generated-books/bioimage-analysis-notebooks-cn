# 生物图像分析笔记本
[![DOI](https://zenodo.org/badge/449194300.svg)](https://zenodo.org/badge/latestdoi/449194300)

这个[Python](https://www.python.org/) [jupyter](https://jupyter.org/)笔记本集合是为对使用现代荧光显微镜获得的细胞、组织、类器官和生物体的三维图像分析感兴趣的Python初学者编写的。基本原理在二维图像数据中进行演示,更复杂的例子应用于三维图像数据和时间序列数据集。

本书是为生物学家、生物化学家和生物物理学家编写的。我们介绍了计算机科学家和数据科学家在描述图像分割、科学计算和图像数据科学时使用的技术语言。

如果您发现有改进的空间,请[创建一个github issue](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/issues)和/或考虑[贡献](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/blob/main/CONTRIBUTING.md)。

## 本Jupyter书的结构

本书的章节最初涵盖Python、图像处理和图像分析的基础知识。之后涵盖了更高级的主题,包括机器学习和统计学。章节的顺序反映了典型的图像分析工作流程,从图像可视化、过滤和分割开始,然后是特征提取、表格数据处理、统计、绘图和数据可视化。每一章的开头,介绍了基本术语,并介绍了本章涵盖的所需Python库的安装说明。这些笔记本旨在自包含、自解释和完全可重现。因此,读者可以下载这本Jupyter书并按原样执行所有笔记本。作为一般要求,读者的计算机上应该有一个conda环境,如第一章所述。

## 涵盖的Python库

这些笔记本涵盖了基本的Python主题,然后过渡到标准的图像处理库,如[scikit-image](http://scikit-image.org/)、[scipy](https://scipy.org)和[numpy](https://numpy.org/)。在高级主题中,我们越来越多地使用GPU加速库,如[pyclesperanto](https://github.com/clEsperanto/pyclesperanto_prototype)和[apoc](https://github.com/haesleinhuepf/apoc)。随着内容向三维生物图像处理和生命科学特定的定量分析转移,我们越来越多地使用我们和我们的合作者维护的自定义开源库。

* [aicsimageio](https://github.com/AllenCellModeling/aicsimageio)
* [apoc](https://github.com/haesleinhuepf/apoc)
* [cupy](https://cupy.dev/)
* [czifile](https://pypi.org/project/czifile/)
* [dask](https://dask.org/)
* [dask-image](http://image.dask.org/en/latest/)
* [hdbscan](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
* [langchain](https://python.langchain.com/en/latest/index.html)
* [matplotlib](https://matplotlib.org/)
* [napari](https://napari.org/)
* [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing)
* [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes)
* [napari-process-points-and-surfaces](https://github.com/haesleinhuepf/napari-process-points-and-surfaces)
* [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)
* [numpy](https://numpy.org/)
* [Nyxus](https://nyxus.readthedocs.io/en/latest/)
* [OpenAI API](https://openai.com/blog/openai-api)
* [pandas](https://pandas.pydata.org/)
* [pandasql](https://github.com/yhat/pandasql/)
* [pyclesperanto_prototype](https://github.com/clEsperanto/pyclesperanto_prototype)
* [pycudadecon](https://github.com/tlambert03/pycudadecon)
* [pyncclient](https://github.com/pragmaticindustries/pyncclient)
* [pyocclient](https://github.com/owncloud/pyocclient)
* [readlif](https://github.com/nimne/readlif)
* [RedLionFish](https://github.com/rosalindfranklininstitute/RedLionfish/)
* [scikit-image](http://scikit-image.org/)
* [scikit-learn](https://scikit-learn.org)
* [scipy](https://scipy.org/)
* [seaborn](https://seaborn.pydata.org/)
* [SimpleITK](https://simpleitk.readthedocs.io/en/master/)
* [stackview](https://github.com/haesleinhuepf/stackview)
* [statsmodels](https://www.statsmodels.org/stable/index.html)
* [the-segmentation-game](https://github.com/haesleinhuepf/the-segmentation-game)
* [umap-learn](https://umap-learn.readthedocs.io/en/latest/)
* [vedo](https://vedo.embl.es/)
* [zarr](https://zarr.readthedocs.io/en/stable/)

## 生物图像分析GPT

这个Jupyter笔记本集合用于创建[生物图像分析GPT](https://chat.openai.com/g/g-psAohb1OY-bio-image-analysis),一个专门用Python进行生物图像分析的基于chatGPT的聊天机器人。

## 相关工作

这不是第一个专注于生物图像分析和相关领域的Python Jupyter笔记本和教学材料集合。还有其他令人惊叹的资源,我们也从中学习。此外,我们之前也制作了一些可在线获得的材料,这些材料肯定会与这本Jupyter书有重叠。

### 书面资源

对于喜欢书面教程和可执行Python Jupyter笔记本的读者,以下资源列表可能会感兴趣。

* [Guillaume Witz的用于成像的深度学习](https://github.com/guiwitz/DLImaging)
* [Guillaume Witz的Numpy和Pandas简介](https://github.com/guiwitz/NumpyPandas_course)
* [Guillaume Witz的NEUBIAS Academy @HOME: 使用Python和Jupyter进行交互式生物图像分析](https://github.com/guiwitz/neubias_academy_biapy)
* [英国皇家显微镜学会(IAFIG-RMS)图像分析焦点兴趣小组的Python生物图像分析课程](https://github.com/IAFIG-RMS/Python-for-Bioimage-Analysis)
* [Juan Nunez-Iglesias的科学Python使用](https://github.com/jni/using-python-for-science)
* [NEUBIAS的培训资源](https://neubias.github.io/training-resources/) 
* [Pete Bankhead的生物图像分析简介](https://bioimagebook.github.io/) 
* [Robert Haase的应用生物图像分析讲座材料(2020)](https://git.mpi-cbg.de/rhaase/lecture_applied_bioimage_analysis_2020)
* [Robert Haase和Anna Poetsch的关于计算生物学的生物图像分析、生物统计学、编程和机器学习的讲座材料(2021)](https://github.com/BiAPoL/Bio-image_Analysis_with_Python)
* [Scikit-image的示例图库](https://scikit-image.org/docs/stable/auto_examples/index.html)
* [Sreeni的显微镜学者Python教程](https://github.com/bnsreenu/python_for_microscopists)
* [Stefan van der Walt的Python讲座材料](https://github.com/stefanv/teaching)
* [Talley Lambert为显微镜学者编写的Python介绍](https://github.com/tlambert03/hms_pyintro2)
* [图灵之道](https://the-turing-way.netlify.app/)

### 视频
专注于各种主题,有YouTuber上传关于显微镜、生物图像分析、Python编程和统计学的视频。

* [Dominik Waithe关于生物图像分析和Python的YouTube频道](https://www.youtube.com/user/odlogo)
* [iBiology关注显微镜和生物图像分析的YouTube频道](https://www.youtube.com/c/ibiology)
* [HHMI Janelia光学兴趣小组YouTube频道](https://www.youtube.com/watch?v=stiM1v0oY9c&list=PLqwpOkZ9dxzKUjBx3dyaqjv6igKhGvAOG)
* [MicroCourses关注显微镜和图像形成的YouTube频道](https://www.youtube.com/c/Microcourses/about)
* [NEUBIAS Academy关于生物图像分析工具的YouTube频道](https://youtube.com/neubias)
* [Robert Haase关于生物图像分析的YouTube讲座,(Python从第9课开始)](https://www.youtube.com/playlist?list=PL5ESQNfM5lc7SAMstEu082ivW4BDMvd0U)
* [Sreeni的YouTube频道(前身为显微镜学者Python教程)](https://www.youtube.com/channel/UC34rW-HtPJulxr5wp2Xa04w)
* [StatQuest with Josh Starmer关于统计和机器学习的YouTube频道](https://www.youtube.com/channel/UCtYLUTtgS3k1Fg4y5tAhLbw)

## 材料来源

这个仓库包含从多个来源收集的Jupyter笔记本。它们在这里维护,以生成内容之间关系更加简化的课程材料。如果您对特定主题感兴趣,您可能会在源仓库中找到更新的材料。

* [apoc](https://github.com/haesleinhuepf/apoc)
* [BiaPol博客](https://github.com/biapol/blog)
* [Bio-image_Analysis_with_Python](https://github.com/BiAPoL/Bio-image_Analysis_with_Python)
* [使用Python和Napari进行图像分析 - 2022年亥姆霍兹成像暑期学院](https://github.com/BiAPoL/HIP_Introduction_to_Napari_and_image_processing_with_Python_2022)
* [2022年EPFL的Python和Napari图像数据科学课程](https://github.com/BiAPoL/Image-data-science-with-Python-and-Napari-EPFL2022)
* [label_neighbor_filters](https://github.com/haesleinhuepf/label_neighbor_filters)
* [lecture_applied_bioimage_analysis_2020](https://git.mpi-cbg.de/rhaase/lecture_applied_bioimage_analysis_2020)
* [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing)
* [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes)
* [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)
* [napari-workflow-optimizer](https://github.com/haesleinhuepf/napari-workflow-optimizer)
* [napari-workflows](https://github.com/haesleinhuepf/napari-workflows)
* [on_the_fly_image_processing_napari](https://github.com/BiAPoL/on_the_fly_image_processing_napari)
* [pyclesperanto-prototype](https://github.com/clesperanto/pyclesperanto_prototype/)
* [DIGS-BB / IMPRS 2022年Python定量生物图像分析课程](https://github.com/BiAPoL/Quantitative_Bio_Image_Analysis_with_Python_2022)

## 问题和答案

如果您想讨论这本Jupyter书中的课程,有反馈和/或建议,请在[image.sc](https://image.sc/)上开一个主题并标记@haesleinhuepf。

## 致谢 /  Acknowledgements

We also thank authors who shared their teaching materials openly so that we could reuse and modify them:
* Anna Poetsch, Biotec, TU Dresden
* Dominik Waithe, University of Oxford
* Guillaume Witz, University of Bern
* Johannes Müller, PoL, TU Dresden
* Laura Žigutytė, PoL, TU Dresden
* Pete Bankhead, University of Edinburgh
* Ryan George Savill, MPI-CBG Dresden / PoL, TU Dresden

We want to acknowledge the people who produced the images we are using for demonstration purposes in this Jupyter book.
* Alba Villaronga Luque, MPI-CBG Dresden
* Alexandr Khrapichev, University of Oxford, UK
* Anne Carpenter, Broad Institute, Boston, MA, United States
* Anne Esslinger, Alberti Lab, MPI-CBG, Germany
* Daniela Vorkel, Myers Lab, MPI-CBG / CSBD, Dresden, Germany
* David Legland, INRAE, UR BIA, Nantes, France
* Jean-Karim Hériché, Cell Biology/Biophysics Unit, EMBL Heidelberg, Germany
* Jesse Veenvliet, MPI-CBG Dresden
* Mauricio Rocha Martins, Norden Lab, MPI-CBG, Germany
* Nasreddin Abolmaali, OncoRay, TU Dresden, Germany
* Sascha M. Kuhn, Nadler Lab, MPI-CBG Dresden, Germany
* Theresa Suckert, OncoRay, University Hospital Carl Gustav Carus, TU Dresden
* Tony Collins, the creator of ImageJ for Microscopy


We acknowledge support by the Deutsche Forschungsgemeinschaft under Germany’s Excellence Strategy—EXC2068–Cluster of Excellence Physics of Life of TU Dresden.
This project has been made possible in part by grant numbers 2021-240341, 2021-237734 and 2022-252520 from the Chan Zuckerberg Initiative DAF, an advised fund of the Silicon Valley Community Foundation.

## License

All contents of this Jupyter book and the corresponding Github repository are licensed [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) and 
BSD3 by the [authors and contributors](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/contributors), unless mentioned otherwise.

## Contributing

Please see our [CONTRIBUTING](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/blob/main/CONTRIBUTING.md) guide for details.
