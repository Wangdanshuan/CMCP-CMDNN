# CMCP-CMDNN

## 简介
这是一个基于CMCP和余弦间隔交叉熵的深度神经网络（CMCP-CMDNN）的Python实现。该网络用于解决二分类问题，可以有效地进行特征选择和提升分类性能。
## 功能特点
1. 提出了余弦间隔交叉熵损失函数，增大判别边界的间隔，提高分类准确率。
2. 引入CMCP惩罚，考虑输入特征对第1隐藏层的权重分组结构，实现特征选择。
3. 提供了模型的算法实现，可进行训练和预测。
4. 在模拟数据集上进行了性能测试，验证了特征选择和分类效果。
5. 应用于信贷违约风险预测问题，表现出良好的预测性能。
## 使用说明
1. 克隆项目：
```
git clone https://github.com/Wangdanshuan/CMCP-CMDNN.git
```
2. 进入项目目录，安装依赖库：
```
cd CMCP-CMDNN
pip install -r requirements.txt
```
3. 生成模拟数据集：
```
python data_generator.py
```
4. 训练模型：
```
python train.py
```
5. 测试模型：
```
python test.py
```
6. 应用模型：
```
python apply.py
```
7. 查看结果：
在results目录下查看分类结果和特征选择结果。
## 注意事项
1. 模型代码位于model.py中，包括前向传播、反向传播和预测函数。
2. 损失函数代码位于loss.py中，包括交叉熵损失和余弦间隔交叉熵损失。
3. 惩罚函数代码位于penalty.py中，包括CMCP函数的实现。
4. 优化器代码位于optimizer.py中，实现了近端梯度下降算法。
5. 数据生成代码位于data_generator.py中，可根据需要生成不同维度的模拟数据集。
6. 模型训练代码位于train.py中，实现了模型的训练。
7. 模型测试代码位于test.py中，实现了模型在测试集上的评估。
8. 模型应用代码位于apply.py中，实现了模型在真实数据集上的应用。
9. 结果存储在results目录下。
希望这个项目对您的研究有所帮助！如果有任何问题或建议，请随时提出。
