---
layout:     post
title:      "Towards Metamerism Via Foveated Style Transfer读书笔记"
author:     "JiG"
header-img: "img/post-bg-kuaidi.jpg"
tags: 

  - Visual metamerism
  - ICLR2019_paper
---

 

# Towards Metamerism Via Foveated Style Transfer

[论文地址](https://openreview.net/forum?id=BJzbG20cFQ))

## Abstract

The problem of visual metamerism is defined as finding a family of perceptually indistinguishable, yet physically different images. In this paper, we propose our NeuroFovea metamer model, a foveated  generative model that is based on a mixture of peripheral representations and style transfer forward-pass algorithms. Our gradient-descent free model is parametrized by a foveated VGG19 encoder-decoder which allows us to encode images in high dimensional space and interpolate between the content and texture information with adaptive instance normalization anywhere in the visual field. Our contributions include: 1) A framework for computing metamers that resembles a noisy communication system via a foveated feed forward encoder-decoder network – We observe that metamerism arises as a byproduct of noisy perturbations that partially lie in the perceptual null space; 2) A perceptual optimization scheme as a solution to the hyperparametric nature of our metamer model that requires tuning of the image-texture tradeoff coefficients everywhere in the visual field which are a consequence of internal noise; 3) An ABX psychophysical evaluation of our metamers where we also find that the rate of growth of the receptive fields in our model match V1 for reference metamers and V2 between synthesized samples. Our model also renders metamers at roughly a second, presenting a ×1000 speed-up compared to the previous work, which allows for tractable data-driven metamer experiments.   



## 摘要



视觉同色异谱的问题定义为找到一个在视觉上无法区分但在物理上不同的图像群。在本文中，我们提出了NeuroFovea metamer模型，该foveated（凹？）生成模型基于外围表示和样式传递正向算法的混合。我们的梯度下降自由模型由foveated(凹?)的VGG19编码器-解码器参数化，该模型使我们可以在高维空间中对图像进行编码，并在视野中的任何位置进行自适应实例归一化，在内容和纹理信息之间进行插值。我们的贡献包括：1）用于计算同构异构体的框架，该框架类似于通过集中式前馈编码器/解码器网络的嘈杂通信系统–我们注意到同构异构体是作为噪声扰动的副产品而产生的，该扰动部分位于感知的零空间内； 2）一种感知优化方案，可以解决我们的metomer模型的超参数性质，该方案需要调整内部噪声导致的视野中图像纹理折衷系数； 3）对我们的同聚物的ABX心理物理评估，我们还发现我们模型中感受野的生长速率与参考同聚物符合V1匹配，和合成样品之间符合V2相匹配。我们的模型还以大约一秒钟的时间渲染了同位异构体，与以前的工作相比，它的速度提高了1000倍，从而可以进行易于处理的数据驱动型同聚物实验。



## 模型结构图

<img src='/img/foveated_generative_style_transfer/1.png' width="500px"/>