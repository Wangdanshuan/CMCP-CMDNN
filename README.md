# 基于CMCP和余弦间隔交叉熵的深度神经网络及其应用 (CMCP-CMDNN)

## 简介

在面对高维数据的分类问题时，传统的深度学习方法往往面临特征选择不足和分类边界不明确的问题。本项目旨在实现一个创新的深度神经网络模型，该模型基于复合最小最大凹罚（Composite Minimax Concave Penalty, CMCP）和余弦间隔交叉熵损失函数，专为解决高维数据分类问题而设计。通过引入CMCP，模型能够有效地从高维数据中筛选出最有信息量的特征；而余弦间隔交叉熵损失函数则通过扩大分类边界的间隔来提高分类的准确率和稳健性。该模型特别适用于金融、生物信息学和社会科学等领域，能够为信用风险评估、疾病诊断和社会行为预测等问题提供强大的分析工具。

## 主要特点

- **特征选择性能**：CMCP通过考虑输入特征对第一隐藏层的权重分组结构，有效剔除无关特征及不重要的连接，从而实现了高维数据的有效压缩和特征选择。
- **分类性能改进**：余弦间隔交叉熵损失函数通过引入扩大因子和距离超参数，提高了模型对不同类别间判别边界的间隔，增强了分类的准确性和鲁棒性。
- **广泛的应用场景**：模型在信用贷款违约风险实证研究中展示了其出色的风险指标选择和违约预警能力，验证了其在实际应用中的有效性和可行性。
- **开放性和可扩展性**：代码结构清晰，易于理解和扩展，便于社区贡献和进一步研究。

## 安装

本项目依赖于Python及数个科学计算库，如NumPy、Pandas和PyTorch等。安装前，请确保已经安装了Python环境（推荐使用Python 3.6及以上版本）。通过以下步骤安装所需依赖：

```bash
git clone https://github.com/your-github-repo/cmcp-cmdnn.git
cd cmcp-cmdnn
pip install -r requirements.txt
```

## 使用指南

1. **数据准备**：将您的数据集放置在`data/`目录下，确保数据格式符合模型输入要求。
2. **模型训练**：运行`src/main.py`来开始训练模型。您可以通过修改`config.json`来调整模型参数和训练设置。
3. **结果评估**：训练完成后，模型的性能将通过准确率、F1分数等指标在测试集上进行评估。

详细的使用示例和参数说明，请参考`docs/usage.md`。

## 贡献指南

我们欢迎社区的贡献和反馈。如果您有任何建议、问题或想要贡献代码，请遵循以下步骤：

1. Fork 项目到您的GitHub账户下。
2. 在您的fork版本上创建一个新的分支。
3. 提交您的更改，并创建一个Pull Request到本项目。
4. 您的Pull Request将会被评审，如果被接受，您的贡献将被合并到项目中。

更多详情，请参阅`CONTRIBUTING.md`。

## 引用

如果您在研究中使用了本项目，请考虑引用我们的论文：

```
王小燕, 冮建伟, 徐龙滔. 基于CMCP和余弦间隔交叉熵的深度神经网络及其应用. 数量经济技术经济研究, 2022.
```

## 许可证

本项目采用 [MIT 许可证](LICENSE)。

## 联系方式

如果您有任何问题或建议，请通过以下方式联系我们：

- 邮箱：example@email.com

感谢您对我们项目的兴趣和支持！
