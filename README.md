# 深度学习与代码理解CodeComprehension

## 相关资料

项目[awesome-machine-learning-on-source-code](https://github.com/src-d/awesome-machine-learning-on-source-code)汇集了绝大部分使用深度学习处理代码相关任务的研究和资源，但是基本上已经有将近一年没有更新。

## 我的工作

### 合并表征空间（合并输入输出端的词汇表）
该部分工作主要基于论文[Learning to Generate Pseudo-code from Source Code using Statistical Machine Translation](https://github.com/delihiros/pseudogen)的数据集进行，据我所知，这是使用深度学习解决代码的问题的第一篇论文。

工作期间，同时做了两个将Python抽象语法树可视化的小工具，[pyAST_visualize](https://github.com/WangS16/pyAST_visualize)是对原始库showast的简单修改，[tree_visualize](https://github.com/WangS16/tree_visualize)是完全自己实现的。


### 对抗性攻击
该部分工作主要基于[Code2Vec](https://code2vec.org/)和[Code2Seq](https://code2seq.org/)的工作，两者的基本原理是差不多的。

### 动态网络
该部分工作的灵感主要来自符号数学领域的博士论文研究[Learning Latent Hierarchical Structures via Probabilistic Models and Deep Learning](https://escholarship.org/uc/item/4w44s8sx)的第四部分。

该部分涉及到的工具主要是抽象语法树的处理
* Python主要是ast库以及[Python语言服务](https://docs.python.org/zh-cn/3/library/language.html)下的一些工具，Java沿用了Code2Vec使用的[Javaparaser](http://javaparser.org/)，实际上也有别的解析工具。

已经验证Pytorch可以训练动态网络。

