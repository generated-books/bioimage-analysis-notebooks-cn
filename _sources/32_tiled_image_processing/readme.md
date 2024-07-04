# 图像分块处理

如果图像数据太大而无法装入内存,就有必要将图像分割成多个"块"并单独处理它们。虽然这一步很简单,但将生成的图像块拼接在一起并返回一个大的结果图像可能变得非常具有挑战性。在本节中,我们将详细阐述处理分块图像的多种策略。[dask库](https://docs.dask.org/en/stable/)使处理分块图像变得易于使用。本章首先展示了一个完整的工作流程,展示了dask的实际应用,然后解释了设置适当的工作流程来处理数据的各个步骤。

另请参阅
* Genevieve Buckley关于["dask-image:大数据的分布式图像处理"](https://www.youtube.com/watch?v=MpjgzNeISeI&t=1359s)的演讲(PyConline AU 2020) [幻灯片](https://genevievebuckley.github.io/dask-image-talk-2020/)
* John Kirkham关于["dask image:一个分布式图像处理库"](https://www.youtube.com/watch?v=XGUS174vvLs)的演讲(SciPy 2019)
* [Dask文档](https://docs.dask.org/en/stable/)
* [Dask image文档](http://image.dask.org/en/latest/)
* [Dask示例:图像处理](https://examples.dask.org/applications/image-processing.html)
* https://github.com/VolkerH/DaskFusion