---
extends: _layouts.post
section: content
title: Backtrader 的安装
slug: install-backtrader
date: 2019-03-13
description: Backtrader 的安装
cover_image: /assets/img/post-cover-image-1.png
categories: [backtrader]
---

相较于其他一些量化交易工具来说，安装 Backtrader 是非常简单的，这主要得益于 Backtrader 的实现几乎没有依赖其他包，除了 matplotlib ，在其核心的数据处理与交易模拟撮合相关更是完全自己使用纯 Python 实现，整体上非常干净。

另外，Backtrader 对于 Python 2/3 版本的兼容也做的比较好，当然在我看来，这个意义不大，更多应该是因为历史包袱，作者一路维护升级上来，观察 Backtrader 代码，可以看到一些作者处理 Python 2/3 兼容的方法，对于需要兼容 Python 2/3 的情景也许有些参考价值。

但是，考虑到 matplotlib 当前版本对于 Python 版本的要求，我们还是最好使用最新的 Python 3.7 环境来安装 Backtrader 。

首先用 conda 创建一个 Python 3.7 的环境

```
conda create -n btenv python=3.7
```

然后激活环境

```
conda activate btenv
```

通过 pypi 安装，并且包括 matplotlib ，方便绘图分析

```
pip install backtrader[plotting]
```

好了安装成功。

打开解释器测试一下

```
import backtrader
```
