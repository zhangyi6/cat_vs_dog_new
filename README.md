## 猫狗大战 ##

### 项目目标 
使用深度学习方法识别一张图片是猫还是狗。

* 输入：一张彩色图片
* 输出：是猫还是狗。

### 使用的库 ###
- keras
- numpy
- pandas
- matplotlib

### 数据 ###

此数据集从 kaggle 上下载。[Dogs vs. Cats Redux: Kernels Edition](https://www.kaggle.com/c/dogs-vs-cats-redux-kernels-edition/data)

### AWS ###
由于此项目要求的计算量较大，建议使用亚马逊 p2.xlarge 云服务器来完成该项目

### 方法 ###
本项目使用了迁移学习的方法，通过使用Xception作为基础模型，固定它部分的权重，来大大减小计算复杂度和训练时间，而且可以获得很好的效果

### 训练时间 ###
训练时，采用batch为16，早期停止的方法`patience=2`，训练了20个epoch，总共耗时5152秒

### 项目结果 ###

本项目的最低要求是 kaggle Public Leaderboard 前 10%。

参考链接：[https://www.kaggle.com/c/dogs-vs-cats-redux-kernels-edition/leaderboard](https://www.kaggle.com/c/dogs-vs-cats-redux-kernels-edition/leaderboard)

用该项目提供的方法，最终得到的结果为**0.04273**，满足项目要求
