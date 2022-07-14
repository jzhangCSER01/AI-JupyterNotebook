### 欠拟合与过拟合

<img src="C:\Users\张炯\AppData\Roaming\Typora\typora-user-images\image-20220713195324821.png" alt="image-20220713195324821" style="zoom:67%;" />

#### 如何解决过拟合问题

原因：

模型结构过于复杂（维度过高）

使用了过多属性，模型训练时包含了干扰信息

解决办法：

简化模型结构（使用低阶模型，比如线性模型）

数据预处理，保留主成分信息（数据PCA处理）

在模型训练时，增加正则化项（regularization）

### 分离训练数据与测试数据

1、把数据分成两部分：训练集、测试集

2、使用训练集数据进行模型训练

3、使用测试集数据进行预测，更有效地评估模型对于新数据的预测表现

### 混淆矩阵(Confusion Matrix)

混淆矩阵，又称误差矩阵，用于衡量分类算法的准确程度

<img src="C:\Users\张炯\AppData\Roaming\Typora\typora-user-images\image-20220713215601756.png" alt="image-20220713215601756" style="zoom:67%;" />

通过混淆矩阵，计算更丰富的模型评估指标

<img src="C:\Users\张炯\AppData\Roaming\Typora\typora-user-images\image-20220713215745734.png" alt="image-20220713215745734" style="zoom:67%;" />

### 模型优化

目标：在确定模型类别后，如何让模型表现更好

三方面：数据、模型核心参数、正则化