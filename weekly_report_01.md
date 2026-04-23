# GNNLearn Weekly Report 01

## Links
- [GNNLearn](https://github.com/lc175/GNNLearn)
- [Graph neural networks: A review of methods and applications](https://doi.org/10.1016/j.aiopen.2021.01.001)

## Done
- 理论学习：复习了图的基本表示（邻接矩阵、度矩阵、拉普拉斯矩阵）和核心概念（节点、边、特征）。阅读了关于 GNN 的综述《Graph neural networks: A review of methods and applications》，初步理解了 GNN 的基本思想、通用设计流程，以及它在图数据任务中的作用。通过 PyG 官网、GNN 101 等资源进一步加深理解。
- 代码实践：安装了 PyTorch Geometric（PyG）框架，加载经典数据集 Cora，并使用 networkx 完成局部图结构可视化。
- 阅读总结：GNN 主要面向非欧几里得数据，可用于节点、边、图等不同层面的任务。其核心是消息传递机制，通常需要结合图类型、数据规模和损失函数进行设计。目前已经建立了较完整的基础知识框架。

## To-Do
- 理论学习：阅读 GCN 原文，进一步理解 GCN 如何聚合邻居节点特征并更新自身表示；继续阅读综述，补充对计算模块、图类型和规模、损失函数设计的理解。
- 动手实践：使用 PyG 实现经典 GCN，在 Cora 数据集上完成节点分类任务。

## Question
- GNN 的工作原理相较于 CNN 更抽象，主要原因在于图数据不如图像或文本直观，因此目前对其消息传递机制的理解还不够完整。
