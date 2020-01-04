---
layout:     post
title:      "AdaIN_style_transfer读书笔记"
author:     "JiG"
header-img: "img/post-bg-kuaidi.jpg"
tags: 

  - Visual metamerism
  - ICCV2017_paper
---

 

# Arbitrary Style Transfer in Real-time with Adaptive Instance Normalization

[论文地址](https://openreview.net/forum?id=BJzbG20cFQ))

## Abstract

Gatys et al. recently introduced a neural algorithm that renders a content image in the style of another image, achieving so-called style transfer. However, their framework requires a slow iterative optimization process, which limits its practical application. Fast approximations with feed-forward neural networks have been proposed to speed up neural style transfer. Unfortunately, the speed improvement comes at a cost: the network is usually tied to a fixed set of styles and cannot adapt to arbitrary new styles. In this paper, we present a simple yet effective approach that for the first time enables arbitrary style transfer in real-time. At the heart of our method is a novel adaptive instance normalization (AdaIN) layer that aligns the mean and variance of the content features with those of the style features. Our method achieves speed comparable to the fastest existing approach, without the restriction to a pre-defined set of styles. In addition, our approach allows flexible user controls such as content-style trade-off, style interpolation, color & spatial controls, all using a single feed-forward neural network.  

## 摘要

Gatys等人最近推出了一种神经算法，可以以另一幅图像的样式呈现内容图像，从而实现所谓的风格迁移。但是，它们的框架要求缓慢的迭代优化过程，这限制了其实际应用。已经提出使用前馈神经网络进行快速逼近，以加快神经样式的传递。不幸的是，提高速度是有代价的：网络通常绑定到一组固定的样式，并且无法适应任意新样式。在本文中，我们提出了一种简单而有效的方法，该方法首次实现了实时的任意样式转换。我们方法的核心是新颖的自适应实例规范化（AdaIN）层，该层将内容特征的均值和方差与样式特征的均值和方差对齐。我们的方法可以达到与现有最快方法相当的速度，而无需限制一组预定义的样式。此外，我们的方法允许使用单个前馈神经网络灵活地进行用户控件，例如内容风格的权衡，风格插值，颜色和空间控件。



## 模型结构图

<img src='/img/AdaIN/1.png' width="500px"/>