---
title: Mid-Term Report
tags: Adervasarial-Training
date: 2021-03-24
status: ongoing
---
# Research on Methods of Accelerating Adversarial Training
 加速对抗训练的方法探究

## 课题简介

{:.boxit}
基于PGD的对抗训练过程是目前最好的防御方法之一，但是对抗训练需要在每次迭代过程生成对抗样本导致其计算资源消耗远大于标准的训练。为了优化对抗训练过程，在保证对抗鲁棒性不受影响的情况下，尽可能减小计算资源消耗，常见的方法有复用生成对抗样本过程的梯度信息，缩短迭代步数等等。本课题旨在综合之前的加速方式并进一步优化对抗训练过程。

## 时间安排

- 1月11日~2月28日：熟悉pytorch框架，关于对抗攻击和防御的基本概念，如FGSM，PGD等
- 3月1日~4月30日：编程实现算法，做实验，调试改进算法
- 5月1日~5月31日：撰写毕业论文

## 文献检索综述

{:.boxit}
通过检索工具查找：在Google搜索、Google学术、aXiv、Web of Science、知网上以Adversarial training, Adversarial attack为关键词进行查找
通过文献参考与引用查找：通过Google学术可以查看已找到文献的引用与被引用，通过在引用与被引用中查找与课题相关的文献

- [1] Adversarial Training for Free! 
- [2] FAST IS BETTER THAN FREE: REVISITING ADVERSARIAL TRAINING
- [3] Towards Deep Learning Models Resistant to Adversarial Attacks

## 项目执行情况
- 1月份到2月份主要在补机器学习和深度学习的背景知识，因为一开始看到的材料很多是使用tensorflow的实现的所以先学了一些tensorflow的框架，实现了一个很粗糙的股票预测模型（顺便找了份实习，这是测试期的工作）。
- 2月底三月初开始一边学习pytorch框架一边了解对抗训练这个领域。
- 学习Pytorch过程
  - 先尝试着编写了一个预测MNIST数据集的Logistic Regression模型，然后改进到用CNN实现。
  - 学习NLP，根据[Simple Word Embedding Model](http://people.ee.duke.edu/~lcarin/acl2018_swem.pdf) (SWEM, Shen et al. 2018)用pytorch框架对实现一组电影评论的情感分析。
- 了解对抗训练
  - 对抗样本[Intriguing properties of neural networks](https://arxiv.org/pdf/1312.6199v4.pdf)
  - 攻击模式
    - 黑盒/白盒；有目标/无目标
  - 对抗样本生成方式
    - FGSM的提出 [Explaining and Harnessing Adversarial Examples](https://arxiv.org/pdf/1412.6572.pdf)
    - I-FGSM [Adversarial examples in the physical world](https://arxiv.org/abs/1607.02533v4)
    - Deepfool [DeepFool: A Simple and Accurate Method to Fool Deep Neural Networks](https://www.cv-foundation.org/openaccess/content_cvpr_2016/html/Moosavi-Dezfooli_DeepFool_A_Simple_CVPR_2016_paper.html)
    - C&W [Towards Evaluating the Robustness of Neural Networks](https://arxiv.org/abs/1608.04644v2)
    - BIM [Adversarial Machine Learning at Scale](https://arxiv.org/abs/1611.01236)
    - PGD，对抗训练Min-Max最优化框架 [Towards Deep Learning Models Resistant to Adversarial Attacks](https://arxiv.org/abs/1706.06083)
    - FreeAT [Adversarial Training for Free!](https://arxiv.org/abs/1904.12843)
    - YOPO [You Only Propagate Once: Accelerating Adversarial Training via Maximal Principle](https://arxiv.org/abs/1905.00877)
    - FreeLB [FREELB: ENHANCED ADVERSARIAL TRAINING FOR NATURAL LANGUAGE UNDERSTANDING](https://iclr.cc/virtual_2020/poster_BygzbyHFvB.html)
  - 防御方法
    - 对抗训练，梯度掩码，随机化，去噪
  - 对抗攻击研究领域
    - 用对抗样本来提升模型的泛化性
    - 改进对抗训练: 对抗训练是目前提高模型鲁棒性最好的方法，但它的缺点也很多，e.g. 速度慢， 在小数据集上训练会overfitting, etc.
      - 加速工作 见上文FreeAT和YOPO
      - 解决overfitting工作 [ADVERSARIALLY ROBUST GENERALIZATION JUST REQUIRES MORE UNLABELED DATA](https://arxiv.org/pdf/1906.00555.pdf)
      - Loss Design角度 [Theoretically Principled Trade-off between Robustness and Accuracy](https://arxiv.org/pdf/1901.08573.pdf)
      - Network architecture design [When NAS Meets Robustness: In Search of Robust Architectures against Adversarial Attacks](https://arxiv.org/pdf/1911.10695.pdf)，[Feature Denoising for Improving Adversarial Robustness](https://arxiv.org/pdf/1812.03411.pdf)角度提升对抗训练性能
    - 除对抗训练之外的方法去提升模型鲁棒性
    - 可迁移对抗样本的产生与理解
    - 模型的可解释性



<!-- 
## 项目存在问题
1. 之前基础打得不是很好，有些过于理论的paper数学部分看起来比较吃力。
2. 拖延症比较严重再加上实习工作和申请材料之类的事情比较占用时间所以对毕设没有很上心，导致项目进度落后了。机器学习这方面背景知识和对抗训练的论文漫无目的的看了一些，比较随意。应该先想清楚具体要选择哪种加速方式进行深入研究，在考虑怎么优化。
3. pytorch虽然研究了一部分，但算法编程这块事实上还没有开始，暂时还在阅读其他人写的开源代码，所以还说不出有什么问题。

## 下一步工作计划
1. 挑重点重读几篇相关论文并研究源码，比如[free_adv_train](https://github.com/ashafahi/free_adv_train). 尝试复现并思考有没有什么地方可以优化的。
2. 编程实现自己的model，调试代码，和现存论文结果进行比较。
3. 差不多有结果后开始撰写毕业论文。 -->