# 算法验证

本章我们将探讨确定分割质量和斑点检测算法质量的技术。

## 另请参阅
* [方法比较研究分析（D.G. Altman 和 J.M. Bland 1983）](https://www-users.york.ac.uk/~mb55/meas/ab83.pdf)
* [方法比较和Bland-Altman图](https://www.youtube.com/watch?v=PbSrSupnZFQ)
* [Sklearn：指标和评分](https://scikit-learn.org/stable/modules/model_evaluation.html)
* [Lena Maier-Hein, Annika Reinke等人. 重新审视指标：图像分析验证的陷阱和建议](https://arxiv.org/abs/2206.01653)
* [（基准）标记：AI验证中的陷阱 | Annika Reinke](https://www.youtube.com/watch?v=HnRcKln5amw)
* [分割结果质量保证博客文章](https://focalplane.biologists.com/2023/04/13/quality-assurance-of-segmentation-results/)

## 安装要求

本章我们将使用[statsmodels库](https://www.statsmodels.org/stable/index.html)进行统计测试。
你可以使用mamba/conda或pip安装它：

```
mamba install -c conda-forge statsmodels
```

```
pip install statsmodels
```