# GNNLearn

本项目用于学习图神经网络（GNN）的基础概念，并结合 PyTorch Geometric（PyG）完成经典数据集的读取与可视化。

当前已完成的内容主要包括：
- 使用 PyTorch Geometric 加载经典引文网络数据集 Cora
- 使用 networkx 和 matplotlib 对局部图结构进行可视化

## 项目结构

```text
GNNLearn/
├─ Cora_networks.ipynb     # Cora 数据集读取与局部图可视化
├─ data/                   # 数据集下载与缓存目录
├─ requirements.txt        # 项目依赖
└─ README.md               # 项目说明
```

## 环境依赖

建议使用 Python 3.10 及以上版本。

安装依赖：

```bash
pip install -r requirements.txt
```

## 主要依赖说明

- `torch`：PyTorch 深度学习框架
- `torch-geometric`：图神经网络相关工具库
- `networkx`：图数据处理与可视化辅助
- `matplotlib`：绘图库
- `jupyter` / `notebook`：运行 notebook 文件


## Notebook 内容说明

`Cora_networks.ipynb` 目前主要完成了以下任务：

1. 导入相关库
2. 加载 Cora 数据集
3. 查看数据集的类别数、特征维度及训练/验证/测试集划分
4. 将 PyG 的图数据转换为 networkx 图对象
5. 选取目标节点，并提取其 1-hop 与 2-hop 邻域
6. 对局部子图进行可视化，并高亮目标节点

## 当前可视化说明

为了适配深色背景环境，notebook 中对图像显示做了如下调整：
- 使用黑色背景
- 使用白色边以增强可见性
- 对目标节点进行红色高亮显示

## 说明

本项目目前以学习记录和基础实验为主，内容会随着后续学习持续补充和完善。
