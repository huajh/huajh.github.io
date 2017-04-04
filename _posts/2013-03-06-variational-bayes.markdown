---
layout: post
title: Variational Bayes
tags:
  - Approximation
  - Determine methods
  - KL Divergence
  - Machine Learning
  - Mean field Method
  - Variational Inference
author: "huajh7"
permalink: "variational-bayes" 
header-img: "img/post-bg-2015.jpg"
date: 2013-03-06 17:34:54
---

***关键词***
 **贝叶斯推断，平均场理论，变分估计，贝叶斯推断，KL散度，确定性估计

* TOC
{:toc}
一、前言

上世纪90年代，变分推断在概率模型上得到迅速发展，在贝叶斯框架下一般的变分法由Attias的两篇文章给出。Matthew J.Beal的博士论文《Variational Algorithms for Approximate Bayesian Inference》中有比较充分地论述，作者将其应用于隐马尔科夫模型，混合因子分析，线性动力学，图模型等。变分贝叶斯是一类用于贝叶斯估计和机器学习领域中近似计算复杂（intractable）积分的技术。它主要应用于复杂的统计模型中，这种模型一般包括三类变量：观测变量(observed variables, data)，未知参数（parameters）和潜变量（latent variables）。在贝叶斯推断中，参数和潜变量统称为不可观测变量(unobserved variables)。变分贝叶斯方法主要是两个目的:

(1)   近似不可观测变量的后验概率，以便通过这些变量作出统计推断。

(2)   对一个特定的模型，给出观测变量的边缘似然函数（或称为证据，evidence）的下界。主要用于模型的选择，认为模型的边缘似然值越高，则模型对数据拟合程度越好，该模型产生Data的概率也越高。

对于第一个目的，蒙特卡洛模拟，特别是用Gibbs取样的MCMC方法，可以近似计算复杂的后验分布，能很好地应用到贝叶斯统计推断。此方法通过大量的样本估计真实的后验，因而近似结果带有一定的随机性。与此不同的是，变分贝叶斯方法提供一种局部最优，但具有确定解的近似后验方法。

从某种角度看，变分贝叶斯可以看做是EM算法的扩展，因为它也是采用极大后验估计(MAP)，即用单个最有可能的参数值来代替完全贝叶斯估计。另外，变分贝叶斯也通过一组相互依然（mutually dependent）的等式进行不断的迭代来获得最优解。

二、问题描述

重新考虑一个问题：1）有一组观测数据$D$，
并且已知模型的形式，求参数与潜变量（或不可观测变量）$$Z = \{ {Z_1},...,{Z_n}\}$$ 的后验分布:$$P(Z|D)$$。

\begin{equation} \label{beta_Gamma}
P(\beta_k) = \mathcal{G}(c_0,d_0), \forall k.
\end{equation}

对于问题一，幸运的是，我们不需要重新定义一个度量指标。在信息论中，已经存在描述两个随机分布之间距离的度量，即相对熵，或者称为Kullback-Leibler散度。


三、Kullback-Leibler散度

[![vb-1](http://blog.huajh7.com/wp-content/uploads/2013/03/vb-1-300x235.png)](http://blog.huajh7.com/2013/03/06/variational-bayes/vb-1/)

四、平均场理论（Mean Field Method）

数学上说，平均场的适用范围只能是完全图，或者说系统结构是well-mixed，在这种情况下，系统中的任何一个个体以等可能接触其他个体。反观物理，平均场与其说是一种方法，不如说是一种思想。其实统计物理的研究目的就是期望对宏观的热力学现象给予合理的微观理论。物理学家坚信，即便不满足完全图的假设，但既然这种“局部”到“整体”的作用得以实现，那么个体之间的局部作用相较于“全局”的作用是可以忽略不计的。


注意这里并非一个不可观测变量一个划分，而应该根据实际情况做决定。当然你也可以这么做，但是有时候，将几个潜变量放在一起会更容易处理。





参考文献

[1] Smídl, Václav, and Anthony Quinn. _The variational Bayes method in signal processing_. Springer, 2006.

[2] Beal, Matthew James. _Variational algorithms for approximate Bayesian inference_. Diss. University of London, 2003.

[3] Fox, Charles W., and Stephen J. Roberts. "A tutorial on variational Bayesian inference." _Artificial Intelligence Review_ 38.2 (2012): 85-95.

[4] Attias, Hagai. "Inferring parameters and structure of latent variable models by variational Bayes." _Proceedings of the Fifteenth conference on Uncertainty in artificial intelligence_. Morgan Kaufmann Publishers Inc., 1999.

[5] Attias, Hagai. "A variational Bayesian framework for graphical models."_Advances in neural information processing systems_ 12.1-2 (2000): 209-215.

全文下载：[**Variational Inference -full.pdf**](http://blog.huajh7.com/wp-content/uploads/2013/03/Variational-Inference-full.pdf)[
](http://blog.huajh7.com/wp-content/uploads/2013/03/Variational-Inference1.pdf)

 