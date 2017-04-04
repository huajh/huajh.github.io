---
layout:     post
title: 		"分布式变分贝叶斯 "
subtitle:   "Distributed Variational Bayesian Algorithms over Sensor Networks"
author:     "huajh7"
catalog:    true
header-img: "img/post-bg-universe.jpg"
tags:
  - Machine Learning
  - Variational Inference
date: 2016-12-15 
---




## Paper

**Hunhao Hua**, Chunguang Li*, [Distributed Variational Bayesian Algorithms over Sensor Networks](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=7303974), IEEE Transactions on Signal Processing, vol.64, no.3, pp.783-798, Feb. 2016. [[PDF]](http://huajh7.com/publications/dVB_hua2016TSP.pdf)

 

## Abstract 

Distributed inference/estimation in Bayesian framework in the context of sensor networks has recently received much attention due to its broad applicability. The variationalBayesian (VB) algorithm is a technique for approximating intractable integrals arising in Bayesian inference. In this paper, we propose two novel distributed VB algorithms for general Bayesian inference problem, which can be applied to a very general class of conjugate-exponential models. In the first approach, the global natural parameters at each node are optimized using a stochastic natural gradient that utilizes the Riemannian geometry of the approximation space, followed by an information diffusion step for cooperationwiththeneighbors.Inthesecond method, a constrained optimization formulation for distributed estimation is established in natural parameter space and solved by alternating direction method of multipliers (ADMM). An application of the distributed inference/estimation of a Bayesian Gaussian mixture model is then presented, to evaluate the effectiveness of the proposed algorithms. Simulations on both synthetic and real datasets demonstrate that the proposed algorithms have excellent performance, which are almost as good as the corresponding centralized VB algorithm relying on all data available in a fusion center.

**Index Terms**-

Alternating direction method of multipliers, distributed algorithm, stochastic natural gradient, variational Bayes,
wireless sensor network (WSN).
 